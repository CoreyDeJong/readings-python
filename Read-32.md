## Django REST Framework Permissions
 - Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.
 - The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user. This corresponds to the IsAuthenticated class in REST framework.
 - The request was successfully authenticated, but permission was denied. — An HTTP 403 Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An HTTP 403 Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. — An HTTP 401 Unauthorized response, with an appropriate WWW-Authenticate header will be returned.
- The AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.
- The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise. This permission is suitable if you want your API to only be accessible to registered users.
- The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.