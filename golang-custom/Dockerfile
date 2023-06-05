FROM golang:latest AS deploy

RUN go install github.com/forestgiant/sliceutil@v0.0.0-20160425183142-94783f95db6c && \
go install github.com/gin-gonic/gin@v1.9.0 && \
go install github.com/swaggo/swag@v1.8.12 && \
go install github.com/tbaehler/gin-keycloak@v1.3.0 && \
go install github.com/bytedance/sonic@v1.8.0 && \
go install github.com/chenzhuoyu/base64x@v0.0.0-20221115062448-fe3a3abad311 && \
go install github.com/google/uuid@v1.1.2 && \
go install github.com/klauspost/cpuid/v2@v2.0.9 && \
go install github.com/twitchyliquid64/golang-asm@v0.15.1 && \ 
go install github.com/KyleBanks/depth@v1.2.1 && \
go install github.com/davecgh/go-spew@v1.1.1 && \
go install github.com/emicklei/go-restful/v3@v3.10.2 && \
go install github.com/gin-contrib/sse@v0.1.0 && \
go install github.com/go-logr/logr@v1.2.4 && \ 
go install github.com/go-openapi/jsonpointer@v0.19.6 && \
go install github.com/go-openapi/jsonreference@v0.20.2 && \
go install github.com/go-openapi/spec@v0.20.8 && \
go install github.com/go-openapi/swag@v0.22.3 && \
go install github.com/go-playground/locales@v0.14.1 && \
go install github.com/go-playground/universal-translator@v0.18.1 && \
go install github.com/go-playground/validator/v10@v10.12.0 && \
go install github.com/goccy/go-json@v0.10.2 && \
go install github.com/gogo/protobuf@v1.3.2 && \
go install github.com/golang/glog@v1.1.1 && \
go install github.com/golang/protobuf@v1.5.3 && \
go install github.com/google/gnostic@v0.6.9 && \
go install github.com/google/go-cmp@v0.5.9 && \
go install github.com/google/gofuzz@v1.2.0 && \
go install github.com/josharian/intern@v1.0.0 && \
go install github.com/json-iterator/go@v1.1.12 && \
go install github.com/leodido/go-urn@v1.2.3 && \
go install github.com/mailru/easyjson@v0.7.7 && \
go install github.com/mattn/go-isatty@v0.0.18 && \
go install github.com/modern-go/concurrent@v0.0.0-20180306012644-bacd9c7ef1dd && \
go install github.com/modern-go/reflect2@v1.0.2 && \
go install github.com/munnerz/goautoneg@v0.0.0-20191010083416-a7dc8b61c822 && \
go install github.com/patrickmn/go-cache@v2.1.0+incompatible && \
go install github.com/pelletier/go-toml/v2@v2.0.7 && \
go install github.com/szuecs/gin-glog@v1.1.1 && \
go install github.com/ugorji/go/codec@v1.2.11 && \
go install golang.org/x/arch@v0.0.0-20210923205945-b76863e36670 && \
go install golang.org/x/crypto@v0.7.0 && \
go install golang.org/x/net@v0.9.0 && \
go install golang.org/x/oauth2@v0.6.0 && \
go install golang.org/x/sys@v0.7.0 && \
go install golang.org/x/term@v0.7.0 && \
go install golang.org/x/text@v0.9.0 && \
go install golang.org/x/time@v0.3.0 && \
go install golang.org/x/tools@v0.7.0 && \
go install google.golang.org/appengine@v1.6.7 && \
go install google.golang.org/protobuf@v1.30.0 && \
go install gopkg.in/inf.v0@v0.9.1 && \
go install gopkg.in/square/go-jose.v2@v2.6.0 && \
go install gopkg.in/yaml.v2@v2.4.0 && \
go install gopkg.in/yaml.v3@v3.0.1 && \
go install k8s.io/klog/v2@v2.90.1 && \
go install k8s.io/kube-openapi@v0.0.0-20230327201221-f5883ff37f0c && \
go install k8s.io/utils@v0.0.0-20230406110748-d93618cff8a2 && \
go install k8s.io/api@v0.26.3 && \
go install k8s.io/apimachinery@v0.26.3 && \
go install k8s.io/client-go@v0.26.3 && \
go install sigs.k8s.io/json@v0.0.0-20221116044647-bc3834ca7abd && \
go install sigs.k8s.io/structured-merge-diff/v4@v4.2.3 && \
go install sigs.k8s.io/yaml@v1.3.0

RUN go mod tidy