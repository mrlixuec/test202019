<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link href="/css/style.css" rel="stylesheet">
<link href="/css/bootstrap.min.css" rel="stylesheet">
    <script src="/js/bootstrap.min.js"></script>
  </head>
  <body>
	
<img src="/pic/banner2.PNG" alt="" class="mb3">
<h2>重要新闻板块的内容</h2>
	{{partial "pagination.html" . }}
  {{ range .Paginator.Pages }}
           
          <div style="border: 1px solid black; margin:10px; padding:10px; ">
               <div style="font-size:20px;">
                    <a href="{{.URL}}">{{.Title}}</a>         {{ .Date  }}
               </div>
       
          </div>
     {{ end }}


  </body>
</html>
