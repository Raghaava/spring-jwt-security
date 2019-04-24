# spring-jwt-security

Implemented blog example from https://dev.to/keysh/spring-security-with-jwt-3j76.

<code>
curl -i -X POST 'http://localhost:8080/api/authenticate?user=admin&pass=admin'
HTTP/1.1 200
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpc3MiOiJzZWN1cmUtYXBpIiwiYXVkIjoic2VjdXJlLWFwcCIsInN1YiI6ImFkbWluIiwiZXhwIjoxNTU2OTU2MTA5LCJyb2wiOlsiUk9MRV9yb2xlX2FkbWluMSJdfQ.hCCqfUwxIFW104lqh8d5ankMewg-n1boIfi1aM0h3FyJ1jCEy5bOJ77h0YgPVM15WOaixf_tWZ-Wcokcb3yCgQ
X-Content-Type-Options: nosniff
X-XSS-Protection: 1; mode=block
Cache-Control: no-cache, no-store, max-age=0, must-revalidate
Pragma: no-cache
Expires: 0
X-Frame-Options: DENY
Content-Length: 0
Date: Wed, 24 Apr 2019 07:48:29 GMT
</code>

<code>
curl -i 'http://localhost:8080/api/private' -H "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpc3MiOiJzZWN1cmUtYXBpIiwiYXVkIjoic2VjdXJlLWFwcCIsInN1YiI6ImFkbWluIiwiZXhwIjoxNTU2OTU0OTkxLCJyb2wiOlsiUk9MRV9yb2xlX2FkbWluMSJdfQ.LiUG53INTR1Cd81LZV57Jgfw1iTPrYSn8kB_Y9tE2hQE7M_S3tBFVf4n1aANNbrnfMxN3kDKvKHMEOjF3JEvvw"
</code>

<code>
curl -i 'http://localhost:8080/api/public
</code>

<B>Resources:</B>
Servlet filters: https://stackoverflow.com/questions/25196867/how-filter-chain-invocation-works
