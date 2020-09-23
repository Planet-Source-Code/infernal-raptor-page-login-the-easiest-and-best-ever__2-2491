<div align="center">

## Page Login \(The easiest and best ever\!\!


</div>

### Description

The purpose of this code is to let the user protect a web page with this simple code. More usernames and passwords can be added if you want.
 
### More Info
 
It returns the safety and sufficentcy of securing a page.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Infernal Raptor](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/infernal-raptor.md)
**Level**          |Beginner
**User Rating**    |2.6 (26 globes from 10 users)
**Compatibility**  |
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__2-74.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/infernal-raptor-page-login-the-easiest-and-best-ever__2-2491/archive/master.zip)





### Source Code

```
<!-- STEP ONE: Copy this code into the HEAD of your login HTML document -->
<HEAD>
<SCRIPT LANGUAGE="JavaScript">
<!-- Begin
function Login(){
var done=0;
var username=document.login.username.value;
username=username.toLowerCase();
var password=document.login.password.value;
password=password.toLowerCase();
if (username=="member1" && password=="password1") { window.location="page1.html"; done=1; }
if (username=="member2" && password=="password2") { window.location="page2.html"; done=1; }
if (username=="member3" && password=="password3") { window.location="page3.html"; done=1; }
if (done==0) { alert("Invalid login! Try again please."); }
}
// End -->
</SCRIPT>
<!-- STEP TWO: Paste this code into the BODY of your HTML document -->
<BODY>
<center>
<form name=login>
<table width=225 border=1 cellpadding=3>
<tr><td colspan=2><center><font size="+2"><b>Members-Only Area!</b></font></center></td></tr>
<tr><td>Username:</td><td><input type=text name=username></td></tr>
<tr><td>Password:</td><td><input type=text name=password></td></tr>
<tr><td colspan=2 align=center><input type=button value="Login!" onClick="Login()"></td></tr>
</table>
</form>
</center>
Add this line to/ instead of your body tag:
(In a standalone HTML file before your protected page)
<BODY bgcolor=black onload="window.open('fullproof.htm','','halfscreen,scrollbars')">
ADD this script at the bottom of your page, just before your </BODY> tag.
(in the page you want to protect)
<SCRIPT LANGUAGE=JAVASCRIPT>
<!--
var message="ENTER YOUR CUSTOM MESSAGE HERE";
  function click(e) {
    if (document.all) {
      if (event.button == 2) {
      alert(message);
      return false;
    }
  }
    if (document.layers) {
      if (e.which == 3) {
      alert(message);
      return false;
    }
  }
}
  if (document.layers) {
  document.captureEvents(Event.MOUSEDOWN);
}
document.onmousedown=click;
// -->
</SCRIPT>
```

