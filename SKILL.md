# micronaut.http Skill

Use this skill to work with Norm module `micronaut.http` version 6. Use only declarations listed below.

## `micronaut.http`

Source: `HttpHeaders.norm`

### `HttpHeaders`

```norm
interface HttpHeaders extends Headers
```

#### `contains`

```norm
Boolean contains(CharSequence? arg0)
```

Parameters:

- `arg0`: `CharSequence?`

Returns: `Boolean`

#### `contains`

```norm
Boolean contains(String? arg0)
```

Parameters:

- `arg0`: `String?`

Returns: `Boolean`

#### `findFirst`

```norm
Optional<String>? findFirst(CharSequence? arg0)
```

Parameters:

- `arg0`: `CharSequence?`

Returns: `Optional<String>?`

#### `getAuthorization`

```norm
Optional<String>? getAuthorization()
```

Returns: `Optional<String>?`

## `micronaut.http`

Source: `HttpMessage.norm`

### `HttpMessage`

```norm
interface HttpMessage<B> extends MutableAttributeHolder
```

Type parameters:

- `B`

## `micronaut.http`

Source: `HttpMethod.norm`

### `HttpMethod`

```norm
enum HttpMethod
```

#### `CONNECT`

```norm
CONNECT
```

#### `CUSTOM`

```norm
CUSTOM
```

#### `DELETE`

```norm
DELETE
```

#### `GET`

```norm
GET
```

#### `HEAD`

```norm
HEAD
```

#### `OPTIONS`

```norm
OPTIONS
```

#### `PATCH`

```norm
PATCH
```

#### `POST`

```norm
POST
```

#### `PUT`

```norm
PUT
```

#### `TRACE`

```norm
TRACE
```

## `micronaut.http`

Source: `HttpRequest.norm`

### `HttpRequest`

```norm
interface HttpRequest<B> extends HttpMessage<B>
```

Type parameters:

- `B`

#### `getHeaders`

```norm
HttpHeaders? getHeaders()
```

Returns: `HttpHeaders?`

#### `getMethodName`

```norm
String? getMethodName()
```

Returns: `String?`

#### `getPath`

```norm
String? getPath()
```

Returns: `String?`

#### `getUri`

```norm
URI? getUri()
```

Returns: `URI?`

#### `isSecure`

```norm
Boolean isSecure()
```

Returns: `Boolean`

## `micronaut.http`

Source: `HttpResponse.norm`

### `HttpResponse`

```norm
interface HttpResponse<B> extends HttpMessage<B>
```

Type parameters:

- `B`

#### `body`

```norm
B? body()
```

Returns: `B?`

#### `code`

```norm
Integer code()
```

Returns: `Integer`

#### `reason`

```norm
String? reason()
```

Returns: `String?`

#### `status`

```norm
HttpStatus? status()
```

Returns: `HttpStatus?`

### `httpResponseAccepted`

```norm
MutableHttpResponse<T>? httpResponseAccepted<T>()
```

Type parameters:

- `T`

Returns: `MutableHttpResponse<T>?`

### `httpResponseBadRequest`

```norm
MutableHttpResponse<T>? httpResponseBadRequest<T>(T? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `T?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseCreated`

```norm
MutableHttpResponse<T>? httpResponseCreated<T>(T? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `T?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseNoContent`

```norm
MutableHttpResponse<T>? httpResponseNoContent<T>()
```

Type parameters:

- `T`

Returns: `MutableHttpResponse<T>?`

### `httpResponseNotFound`

```norm
MutableHttpResponse<T>? httpResponseNotFound<T>()
```

Type parameters:

- `T`

Returns: `MutableHttpResponse<T>?`

### `httpResponseOk`

```norm
MutableHttpResponse<T>? httpResponseOk<T>()
```

Type parameters:

- `T`

Returns: `MutableHttpResponse<T>?`

### `httpResponseOk`

```norm
MutableHttpResponse<T>? httpResponseOk<T>(T? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `T?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseSeeOther`

```norm
MutableHttpResponse<T>? httpResponseSeeOther<T>(URI? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `URI?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseServerError`

```norm
MutableHttpResponse<T>? httpResponseServerError<T>(T? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `T?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseStatus`

```norm
MutableHttpResponse<T>? httpResponseStatus<T>(Integer arg0, String? arg1)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `Integer`
- `arg1`: `String?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseStatus`

```norm
MutableHttpResponse<T>? httpResponseStatus<T>(HttpStatus? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `HttpStatus?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseStatus`

```norm
MutableHttpResponse<T>? httpResponseStatus<T>(HttpStatus? arg0, String? arg1)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `HttpStatus?`
- `arg1`: `String?`

Returns: `MutableHttpResponse<T>?`

### `httpResponseUnauthorized`

```norm
MutableHttpResponse<T>? httpResponseUnauthorized<T>()
```

Type parameters:

- `T`

Returns: `MutableHttpResponse<T>?`

## `micronaut.http`

Source: `HttpStatus.norm`

### `HttpStatus`

```norm
enum HttpStatus
```

#### `ACCEPTED`

```norm
ACCEPTED
```

#### `ALREADY_IMPORTED`

```norm
ALREADY_IMPORTED
```

#### `BAD_GATEWAY`

```norm
BAD_GATEWAY
```

#### `BAD_REQUEST`

```norm
BAD_REQUEST
```

#### `BANDWIDTH_LIMIT_EXCEEDED`

```norm
BANDWIDTH_LIMIT_EXCEEDED
```

#### `BLOCKED_BY_WINDOWS_PARENTAL_CONTROLS`

```norm
BLOCKED_BY_WINDOWS_PARENTAL_CONTROLS
```

#### `CONFLICT`

```norm
CONFLICT
```

#### `CONNECTION_TIMED_OUT`

```norm
CONNECTION_TIMED_OUT
```

#### `CONTINUE`

```norm
CONTINUE
```

#### `CREATED`

```norm
CREATED
```

#### `EARLY_HINTS`

```norm
EARLY_HINTS
```

#### `ENHANCE_YOUR_CALM`

```norm
ENHANCE_YOUR_CALM
```

#### `EXPECTATION_FAILED`

```norm
EXPECTATION_FAILED
```

#### `FAILED_DEPENDENCY`

```norm
FAILED_DEPENDENCY
```

#### `FORBIDDEN`

```norm
FORBIDDEN
```

#### `FOUND`

```norm
FOUND
```

#### `GATEWAY_TIMEOUT`

```norm
GATEWAY_TIMEOUT
```

#### `GONE`

```norm
GONE
```

#### `HTTP_VERSION_NOT_SUPPORTED`

```norm
HTTP_VERSION_NOT_SUPPORTED
```

#### `IM_USED`

```norm
IM_USED
```

#### `INSUFFICIENT_STORAGE`

```norm
INSUFFICIENT_STORAGE
```

#### `INTERNAL_SERVER_ERROR`

```norm
INTERNAL_SERVER_ERROR
```

#### `I_AM_A_TEAPOT`

```norm
I_AM_A_TEAPOT
```

#### `LENGTH_REQUIRED`

```norm
LENGTH_REQUIRED
```

#### `LOCKED`

```norm
LOCKED
```

#### `LOOP_DETECTED`

```norm
LOOP_DETECTED
```

#### `METHOD_NOT_ALLOWED`

```norm
METHOD_NOT_ALLOWED
```

#### `MISDIRECTED_REQUEST`

```norm
MISDIRECTED_REQUEST
```

#### `MOVED_PERMANENTLY`

```norm
MOVED_PERMANENTLY
```

#### `MULTIPLE_CHOICES`

```norm
MULTIPLE_CHOICES
```

#### `MULTI_STATUS`

```norm
MULTI_STATUS
```

#### `NETWORK_AUTHENTICATION_REQUIRED`

```norm
NETWORK_AUTHENTICATION_REQUIRED
```

#### `NON_AUTHORITATIVE_INFORMATION`

```norm
NON_AUTHORITATIVE_INFORMATION
```

#### `NOT_ACCEPTABLE`

```norm
NOT_ACCEPTABLE
```

#### `NOT_EXTENDED`

```norm
NOT_EXTENDED
```

#### `NOT_FOUND`

```norm
NOT_FOUND
```

#### `NOT_IMPLEMENTED`

```norm
NOT_IMPLEMENTED
```

#### `NOT_MODIFIED`

```norm
NOT_MODIFIED
```

#### `NO_CONTENT`

```norm
NO_CONTENT
```

#### `NO_RESPONSE`

```norm
NO_RESPONSE
```

#### `OK`

```norm
OK
```

#### `PARTIAL_CONTENT`

```norm
PARTIAL_CONTENT
```

#### `PAYMENT_REQUIRED`

```norm
PAYMENT_REQUIRED
```

#### `PERMANENT_REDIRECT`

```norm
PERMANENT_REDIRECT
```

#### `PRECONDITION_FAILED`

```norm
PRECONDITION_FAILED
```

#### `PRECONDITION_REQUIRED`

```norm
PRECONDITION_REQUIRED
```

#### `PROCESSING`

```norm
PROCESSING
```

#### `PROXY_AUTHENTICATION_REQUIRED`

```norm
PROXY_AUTHENTICATION_REQUIRED
```

#### `REQUESTED_RANGE_NOT_SATISFIABLE`

```norm
REQUESTED_RANGE_NOT_SATISFIABLE
```

#### `REQUEST_ENTITY_TOO_LARGE`

```norm
REQUEST_ENTITY_TOO_LARGE
```

#### `REQUEST_HEADER_FIELDS_TOO_LARGE`

```norm
REQUEST_HEADER_FIELDS_TOO_LARGE
```

#### `REQUEST_HEADER_TOO_LARGE`

```norm
REQUEST_HEADER_TOO_LARGE
```

#### `REQUEST_TIMEOUT`

```norm
REQUEST_TIMEOUT
```

#### `REQUEST_URI_TOO_LONG`

```norm
REQUEST_URI_TOO_LONG
```

#### `RESET_CONTENT`

```norm
RESET_CONTENT
```

#### `SEE_OTHER`

```norm
SEE_OTHER
```

#### `SERVICE_UNAVAILABLE`

```norm
SERVICE_UNAVAILABLE
```

#### `SWITCHING_PROTOCOLS`

```norm
SWITCHING_PROTOCOLS
```

#### `SWITCH_PROXY`

```norm
SWITCH_PROXY
```

#### `TEMPORARY_REDIRECT`

```norm
TEMPORARY_REDIRECT
```

#### `TOO_EARLY`

```norm
TOO_EARLY
```

#### `TOO_MANY_REQUESTS`

```norm
TOO_MANY_REQUESTS
```

#### `UNAUTHORIZED`

```norm
UNAUTHORIZED
```

#### `UNAVAILABLE_FOR_LEGAL_REASONS`

```norm
UNAVAILABLE_FOR_LEGAL_REASONS
```

#### `UNPROCESSABLE_ENTITY`

```norm
UNPROCESSABLE_ENTITY
```

#### `UNSUPPORTED_MEDIA_TYPE`

```norm
UNSUPPORTED_MEDIA_TYPE
```

#### `UPGRADE_REQUIRED`

```norm
UPGRADE_REQUIRED
```

#### `USE_PROXY`

```norm
USE_PROXY
```

#### `VARIANT_ALSO_NEGOTIATES`

```norm
VARIANT_ALSO_NEGOTIATES
```

### `httpStatusGetCode`

```norm
Integer httpStatusGetCode(HttpStatus receiver)
```

Parameters:

- `receiver`: `HttpStatus`

Returns: `Integer`

### `httpStatusGetReason`

```norm
String? httpStatusGetReason(HttpStatus receiver)
```

Parameters:

- `receiver`: `HttpStatus`

Returns: `String?`

## `micronaut.http`

Source: `JavaArrays.norm`

### `JavaStringArray`

```norm
class JavaStringArray
```

#### `JavaStringArray`

```norm
JavaStringArray(JavaStringArrayBindingToken token)
```

Parameters:

- `token`: `JavaStringArrayBindingToken`

#### `size`

```norm
Integer size()
```

Returns: `Integer`

#### `get`

```norm
String? get(Integer index)
```

Parameters:

- `index`: `Integer`

Returns: `String?`

#### `set`

```norm
Void set(Integer index, String? value)
```

Parameters:

- `index`: `Integer`
- `value`: `String?`

Returns: `Void`

### `javaStringArrayNew`

```norm
JavaStringArray javaStringArrayNew(Integer size)
```

Parameters:

- `size`: `Integer`

Returns: `JavaStringArray`

### `JavaHttpMethodArray`

```norm
class JavaHttpMethodArray
```

#### `JavaHttpMethodArray`

```norm
JavaHttpMethodArray(JavaHttpMethodArrayBindingToken token)
```

Parameters:

- `token`: `JavaHttpMethodArrayBindingToken`

#### `size`

```norm
Integer size()
```

Returns: `Integer`

#### `get`

```norm
HttpMethod? get(Integer index)
```

Parameters:

- `index`: `Integer`

Returns: `HttpMethod?`

#### `set`

```norm
Void set(Integer index, HttpMethod? value)
```

Parameters:

- `index`: `Integer`
- `value`: `HttpMethod?`

Returns: `Void`

### `javaHttpMethodArrayNew`

```norm
JavaHttpMethodArray javaHttpMethodArrayNew(Integer size)
```

Parameters:

- `size`: `Integer`

Returns: `JavaHttpMethodArray`

## `micronaut.http`

Source: `MutableHttpMessage.norm`

### `MutableHttpMessage`

```norm
interface MutableHttpMessage<B> extends HttpMessage<B>
```

Type parameters:

- `B`

## `micronaut.http`

Source: `MutableHttpResponse.norm`

### `MutableHttpResponse`

```norm
interface MutableHttpResponse<B> extends HttpResponse<B>, MutableHttpMessage<B>
```

Type parameters:

- `B`

## `micronaut.http.annotation`

Source: `annotation/Body.norm`

### `Body`

```norm
annotation Body implements ParameterTarget, RuntimeRetention, InheritedAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `Body`

```norm
Body(String? defaultValue, String? value)
```

Parameters:

- `defaultValue`: `String?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/Consumes.norm`

### `Consumes`

```norm
annotation Consumes implements TypeTarget, FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `value`

```norm
List<String> value
```

Type: `List<String>`

#### `Consumes`

```norm
Consumes(List<String>? value)
```

Parameters:

- `value`: `List<String>?`

## `micronaut.http.annotation`

Source: `annotation/Controller.norm`

### `Controller`

```norm
annotation Controller implements TypeTarget, RuntimeRetention
```

#### `consumes`

```norm
List<String> consumes
```

Type: `List<String>`

#### `port`

```norm
String port
```

Type: `String`

#### `produces`

```norm
List<String> produces
```

Type: `List<String>`

#### `value`

```norm
String value
```

Type: `String`

#### `Controller`

```norm
Controller(List<String>? consumes, String? port, List<String>? produces, String? value)
```

Parameters:

- `consumes`: `List<String>?`
- `port`: `String?`
- `produces`: `List<String>?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/CookieValue.norm`

### `CookieValue`

```norm
annotation CookieValue implements TypeTarget, FieldTarget, ParameterTarget, RuntimeRetention, InheritedAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `CookieValue`

```norm
CookieValue(String? defaultValue, String? value)
```

Parameters:

- `defaultValue`: `String?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/Delete.norm`

### `Delete`

```norm
annotation Delete implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `consumes`

```norm
List<String> consumes
```

Type: `List<String>`

#### `processes`

```norm
List<String> processes
```

Type: `List<String>`

#### `produces`

```norm
List<String> produces
```

Type: `List<String>`

#### `single`

```norm
Boolean single
```

Type: `Boolean`

#### `uri`

```norm
String uri
```

Type: `String`

#### `uris`

```norm
List<String> uris
```

Type: `List<String>`

#### `value`

```norm
String value
```

Type: `String`

#### `Delete`

```norm
Delete(List<String>? consumes, List<String>? processes, List<String>? produces, Boolean? single, String? uri, List<String>? uris, String? value)
```

Parameters:

- `consumes`: `List<String>?`
- `processes`: `List<String>?`
- `produces`: `List<String>?`
- `single`: `Boolean?`
- `uri`: `String?`
- `uris`: `List<String>?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/Error.norm`

### `Error`

```norm
annotation Error implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `exception`

```norm
Class<?> exception
```

Type: `Class<?>`

#### `global`

```norm
Boolean global
```

Type: `Boolean`

#### `status`

```norm
HttpStatus status
```

Type: `HttpStatus`

#### `value`

```norm
Class<?> value
```

Type: `Class<?>`

#### `Error`

```norm
Error(Class<?>? exception, Boolean? global, HttpStatus? status, Class<?>? value)
```

Parameters:

- `exception`: `Class<?>?`
- `global`: `Boolean?`
- `status`: `HttpStatus?`
- `value`: `Class<?>?`

## `micronaut.http.annotation`

Source: `annotation/Get.norm`

### `Get`

```norm
annotation Get implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `consumes`

```norm
List<String> consumes
```

Type: `List<String>`

#### `headRoute`

```norm
Boolean headRoute
```

Type: `Boolean`

#### `processes`

```norm
List<String> processes
```

Type: `List<String>`

#### `produces`

```norm
List<String> produces
```

Type: `List<String>`

#### `single`

```norm
Boolean single
```

Type: `Boolean`

#### `uri`

```norm
String uri
```

Type: `String`

#### `uris`

```norm
List<String> uris
```

Type: `List<String>`

#### `value`

```norm
String value
```

Type: `String`

#### `Get`

```norm
Get(List<String>? consumes, Boolean? headRoute, List<String>? processes, List<String>? produces, Boolean? single, String? uri, List<String>? uris, String? value)
```

Parameters:

- `consumes`: `List<String>?`
- `headRoute`: `Boolean?`
- `processes`: `List<String>?`
- `produces`: `List<String>?`
- `single`: `Boolean?`
- `uri`: `String?`
- `uris`: `List<String>?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/Header.norm`

### `Header`

```norm
annotation Header implements TypeTarget, FieldTarget, FunctionTarget, ParameterTarget, RuntimeRetention, InheritedAnnotation, RepeatableAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

Type: `String`

#### `name`

```norm
String name
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `Header`

```norm
Header(String? defaultValue, String? name, String? value)
```

Parameters:

- `defaultValue`: `String?`
- `name`: `String?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/Patch.norm`

### `Patch`

```norm
annotation Patch implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `consumes`

```norm
List<String> consumes
```

Type: `List<String>`

#### `processes`

```norm
List<String> processes
```

Type: `List<String>`

#### `produces`

```norm
List<String> produces
```

Type: `List<String>`

#### `single`

```norm
Boolean single
```

Type: `Boolean`

#### `uri`

```norm
String uri
```

Type: `String`

#### `uris`

```norm
List<String> uris
```

Type: `List<String>`

#### `value`

```norm
String value
```

Type: `String`

#### `Patch`

```norm
Patch(List<String>? consumes, List<String>? processes, List<String>? produces, Boolean? single, String? uri, List<String>? uris, String? value)
```

Parameters:

- `consumes`: `List<String>?`
- `processes`: `List<String>?`
- `produces`: `List<String>?`
- `single`: `Boolean?`
- `uri`: `String?`
- `uris`: `List<String>?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/PathVariable.norm`

### `PathVariable`

```norm
annotation PathVariable implements TypeTarget, FieldTarget, ParameterTarget, RuntimeRetention, InheritedAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

Type: `String`

#### `name`

```norm
String name
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `PathVariable`

```norm
PathVariable(String? defaultValue, String? name, String? value)
```

Parameters:

- `defaultValue`: `String?`
- `name`: `String?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/Post.norm`

### `Post`

```norm
annotation Post implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `consumes`

```norm
List<String> consumes
```

Type: `List<String>`

#### `processes`

```norm
List<String> processes
```

Type: `List<String>`

#### `produces`

```norm
List<String> produces
```

Type: `List<String>`

#### `single`

```norm
Boolean single
```

Type: `Boolean`

#### `uri`

```norm
String uri
```

Type: `String`

#### `uris`

```norm
List<String> uris
```

Type: `List<String>`

#### `value`

```norm
String value
```

Type: `String`

#### `Post`

```norm
Post(List<String>? consumes, List<String>? processes, List<String>? produces, Boolean? single, String? uri, List<String>? uris, String? value)
```

Parameters:

- `consumes`: `List<String>?`
- `processes`: `List<String>?`
- `produces`: `List<String>?`
- `single`: `Boolean?`
- `uri`: `String?`
- `uris`: `List<String>?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/Produces.norm`

### `Produces`

```norm
annotation Produces implements TypeTarget, FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `value`

```norm
List<String> value
```

Type: `List<String>`

#### `Produces`

```norm
Produces(List<String>? value)
```

Parameters:

- `value`: `List<String>?`

## `micronaut.http.annotation`

Source: `annotation/Put.norm`

### `Put`

```norm
annotation Put implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `consumes`

```norm
List<String> consumes
```

Type: `List<String>`

#### `processes`

```norm
List<String> processes
```

Type: `List<String>`

#### `produces`

```norm
List<String> produces
```

Type: `List<String>`

#### `single`

```norm
Boolean single
```

Type: `Boolean`

#### `uri`

```norm
String uri
```

Type: `String`

#### `uris`

```norm
List<String> uris
```

Type: `List<String>`

#### `value`

```norm
String value
```

Type: `String`

#### `Put`

```norm
Put(List<String>? consumes, List<String>? processes, List<String>? produces, Boolean? single, String? uri, List<String>? uris, String? value)
```

Parameters:

- `consumes`: `List<String>?`
- `processes`: `List<String>?`
- `produces`: `List<String>?`
- `single`: `Boolean?`
- `uri`: `String?`
- `uris`: `List<String>?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/QueryValue.norm`

### `QueryValue`

```norm
annotation QueryValue implements TypeTarget, FieldTarget, ParameterTarget, RuntimeRetention, InheritedAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `QueryValue`

```norm
QueryValue(String? defaultValue, String? value)
```

Parameters:

- `defaultValue`: `String?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/RequestAttribute.norm`

### `RequestAttribute`

```norm
annotation RequestAttribute implements TypeTarget, FunctionTarget, ParameterTarget, RuntimeRetention, RepeatableAnnotation
```

#### `defaultValue`

```norm
String defaultValue
```

Type: `String`

#### `value`

```norm
String value
```

Type: `String`

#### `RequestAttribute`

```norm
RequestAttribute(String? defaultValue, String? value)
```

Parameters:

- `defaultValue`: `String?`
- `value`: `String?`

## `micronaut.http.annotation`

Source: `annotation/RequestBean.norm`

### `RequestBean`

```norm
annotation RequestBean implements TypeTarget, ParameterTarget, RuntimeRetention, InheritedAnnotation
```

## `micronaut.http.annotation`

Source: `annotation/RequestFilter.norm`

### `RequestFilter`

```norm
annotation RequestFilter implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `methods`

```norm
List<HttpMethod> methods
```

Type: `List<HttpMethod>`

#### `patternStyle`

```norm
FilterPatternStyle patternStyle
```

Type: `FilterPatternStyle`

#### `patterns`

```norm
List<String> patterns
```

Type: `List<String>`

#### `value`

```norm
List<String> value
```

Type: `List<String>`

#### `RequestFilter`

```norm
RequestFilter(List<HttpMethod>? methods, FilterPatternStyle? patternStyle, List<String>? patterns, List<String>? value)
```

Parameters:

- `methods`: `List<HttpMethod>?`
- `patternStyle`: `FilterPatternStyle?`
- `patterns`: `List<String>?`
- `value`: `List<String>?`

## `micronaut.http.annotation`

Source: `annotation/ResponseFilter.norm`

### `ResponseFilter`

```norm
annotation ResponseFilter implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `methods`

```norm
List<HttpMethod> methods
```

Type: `List<HttpMethod>`

#### `patternStyle`

```norm
FilterPatternStyle patternStyle
```

Type: `FilterPatternStyle`

#### `patterns`

```norm
List<String> patterns
```

Type: `List<String>`

#### `value`

```norm
List<String> value
```

Type: `List<String>`

#### `ResponseFilter`

```norm
ResponseFilter(List<HttpMethod>? methods, FilterPatternStyle? patternStyle, List<String>? patterns, List<String>? value)
```

Parameters:

- `methods`: `List<HttpMethod>?`
- `patternStyle`: `FilterPatternStyle?`
- `patterns`: `List<String>?`
- `value`: `List<String>?`

## `micronaut.http.annotation`

Source: `annotation/ServerFilter.norm`

### `ServerFilter`

```norm
annotation ServerFilter implements TypeTarget, RuntimeRetention
```

#### `appendContextPath`

```norm
Boolean appendContextPath
```

Type: `Boolean`

#### `methods`

```norm
List<HttpMethod> methods
```

Type: `List<HttpMethod>`

#### `patternStyle`

```norm
FilterPatternStyle patternStyle
```

Type: `FilterPatternStyle`

#### `patterns`

```norm
List<String> patterns
```

Type: `List<String>`

#### `value`

```norm
List<String> value
```

Type: `List<String>`

#### `ServerFilter`

```norm
ServerFilter(Boolean? appendContextPath, List<HttpMethod>? methods, FilterPatternStyle? patternStyle, List<String>? patterns, List<String>? value)
```

Parameters:

- `appendContextPath`: `Boolean?`
- `methods`: `List<HttpMethod>?`
- `patternStyle`: `FilterPatternStyle?`
- `patterns`: `List<String>?`
- `value`: `List<String>?`

## `micronaut.http.annotation`

Source: `annotation/Status.norm`

### `Status`

```norm
annotation Status implements FunctionTarget, RuntimeRetention, InheritedAnnotation
```

#### `value`

```norm
HttpStatus value
```

Type: `HttpStatus`

## `micronaut.http.filter`

Source: `filter/FilterPatternStyle.norm`

### `FilterPatternStyle`

```norm
enum FilterPatternStyle
```

#### `ANT`

```norm
ANT
```

#### `REGEX`

```norm
REGEX
```

## `micronaut.http.io.micronaut.core.attr`

Source: `io/micronaut/core/attr/AttributeHolder.norm`

### `AttributeHolder`

```norm
interface AttributeHolder
```

## `micronaut.http.io.micronaut.core.attr`

Source: `io/micronaut/core/attr/MutableAttributeHolder.norm`

### `MutableAttributeHolder`

```norm
interface MutableAttributeHolder extends AttributeHolder
```

## `micronaut.http.io.micronaut.core.convert`

Source: `io/micronaut/core/convert/ConversionServiceProvider.norm`

### `ConversionServiceProvider`

```norm
interface ConversionServiceProvider
```

## `micronaut.http.io.micronaut.core.convert.value`

Source: `io/micronaut/core/convert/value/ConvertibleMultiValues.norm`

### `ConvertibleMultiValues`

```norm
interface ConvertibleMultiValues<V> extends ConvertibleValues<JavaList<V>>
```

Type parameters:

- `V`

## `micronaut.http.io.micronaut.core.convert.value`

Source: `io/micronaut/core/convert/value/ConvertibleValues.norm`

### `ConvertibleValues`

```norm
interface ConvertibleValues<V> extends ValueResolver<CharSequence>, Iterable<Map_Entry<String, V>>, ConversionServiceProvider
```

Type parameters:

- `V`

## `micronaut.http.io.micronaut.core.type`

Source: `io/micronaut/core/type/Headers.norm`

### `Headers`

```norm
interface Headers extends ConvertibleMultiValues<String>
```

## `micronaut.http.io.micronaut.core.value`

Source: `io/micronaut/core/value/ValueResolver.norm`

### `ValueResolver`

```norm
interface ValueResolver<K extends CharSequence>
```

Type parameters:

- `K` extends `CharSequence`

## `micronaut.http.sse`

Source: `sse/Event.norm`

### `Event`

```norm
interface Event<T>
```

Type parameters:

- `T`

#### `comment`

```norm
Event<T>? comment(String? arg0)
```

Parameters:

- `arg0`: `String?`

Returns: `Event<T>?`

#### `getComment`

```norm
String? getComment()
```

Returns: `String?`

#### `getData`

```norm
T? getData()
```

Returns: `T?`

#### `getId`

```norm
String? getId()
```

Returns: `String?`

#### `getName`

```norm
String? getName()
```

Returns: `String?`

#### `getRetry`

```norm
Duration? getRetry()
```

Returns: `Duration?`

#### `id`

```norm
Event<T>? id(String? arg0)
```

Parameters:

- `arg0`: `String?`

Returns: `Event<T>?`

#### `name`

```norm
Event<T>? name(String? arg0)
```

Parameters:

- `arg0`: `String?`

Returns: `Event<T>?`

#### `retry`

```norm
Event<T>? retry(Duration? arg0)
```

Parameters:

- `arg0`: `Duration?`

Returns: `Event<T>?`

### `eventOf`

```norm
Event<ET>? eventOf<ET>(ET? arg0)
```

Type parameters:

- `ET`

Parameters:

- `arg0`: `ET?`

Returns: `Event<ET>?`

