

# digest
`import "digest"`

* [Overview](#pkg-overview)
* [Index](#pkg-index)

## <a name="pkg-overview">Overview</a>
Packlage digest provides a wrapper for http.Client that supports HTTP Digest
auth for GET and POST (and other) HTTP methods




## <a name="pkg-index">Index</a>
* [type AuthClient](#AuthClient)
  * [func NewAuthClient(c \*http.Client, user, pass string) \*AuthClient](#NewAuthClient)
  * [func (c \*AuthClient) Do(r \*http.Request) (\*http.Response, error)](#AuthClient.Do)


#### <a name="pkg-files">Package files</a>
[digest.go](/src/digest/digest.go) 






## <a name="AuthClient">type</a> [AuthClient](/src/target/digest.go?s=303:377#L6)
``` go
type AuthClient struct {
    *http.Client
    User     string
    Password string
}
```
Type AuthClient is a wrapper around http.Client







### <a name="NewAuthClient">func</a> [NewAuthClient](/src/target/digest.go?s=430:495#L13)
``` go
func NewAuthClient(c *http.Client, user, pass string) *AuthClient
```
NewAuthClient returns a new AuthClient instance





### <a name="AuthClient.Do">func</a> (\*AuthClient) [Do](/src/target/digest.go?s=623:687#L20)
``` go
func (c *AuthClient) Do(r *http.Request) (*http.Response, error)
```
Do performs a request, and performs digeset authentication








- - -
Generated by [godoc2md](http://godoc.org/github.com/davecheney/godoc2md)
