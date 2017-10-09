# Asp.Net-MVC-5-migrate-to-Asp.net-Core-2.0

## 1. class or class member changes
* OutputCache => ResponseCache
* OutputCacheLocation => ResponseCacheLocation
* VaryByParam => VaryByQueryKeys or VaryByHeader 

* Server.MapPath => IHostingEnvironment.WebRootPath  or IHostingEnvironment.ContentRootPath


* Response.OutputStream => Response.Body
* Request.InputStream  => Request.Body

* HttpContext.Request.QueryString.Get() => HttpContext.Request.Query.TryGetValue()

* HttpNotFound => NotFoundObjectResult
* HttpNotFound() => NotFound()
* HttpUnauthorizedResult => UnauthorizedResult

* MemoryCache.Default  => IMemoryCache
* MemoryCache.Default.Set  => _memoryCache.Set<>
* MemoryCache.Default.Get => _memoryCache.TryGetValue<>

## 2. To support WCF, install [WCF Connected Service](https://marketplace.visualstudio.com/items?itemName=erikcai-MSFT.VisualStudioWCFConnectedService) via nuget

## 3. Not .Net Remoting support any more























