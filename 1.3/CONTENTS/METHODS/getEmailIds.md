<a href="/1.3/README.md">Back to the Table of Contents</a>&nbsp;&nbsp;|&nbsp;&nbsp;<a href="API_METHODS.md">Back to API Methods</a>
<h2>getEmailIds</h2>
<p><strong>Synopsis:</strong><br />
This API function returns a comma separated list of Email Template Ids for that account. </p>
<div><strong>Request: XML</strong></div>
<pre>&lt;REQUEST&gt;
    &lt;ACTION&gt;getEmailIds&lt;/ACTION&gt;
    &lt;API_KEY&gt;apiKey&lt;/API_KEY&gt;
&lt;/REQUEST&gt;</pre>
<div><strong>Request: GET</strong></div>
<pre>API_URL?action=getemailids&amp;api_key=apiKey</pre>
<div><strong>Request Parameters:</strong></div>
<pre><strong>Mandatory:</strong>
action, apikey
<strong>Optional:</strong>
--
</pre>

<strong>Response Parameters:</strong><br />
status, emailids, Errorcode, Errorinfo

<strong>Related Errorcodes: </strong><br />
E400
<div><strong>Request Examples</strong></div>
XML:
<pre>&lt;REQUEST&gt;
    &lt;ACTION&gt;getEmailIds&lt;/ACTION&gt;
    &lt;API_KEY&gt;qTFkykO9JTfahCOqJ0V2Wf5Cg1t8iWlZ&lt;/API_KEY&gt;    
&lt;/REQUEST&gt;</pre>
GET:
<pre>https://secure.skycore.com/API/wxml/1.3/index.php?action=getemailids&api_key=qTFkykO9JTfahCOqJ0V2Wf5Cg1t8iWlZ</pre>
<div><strong>Response Example: Success</strong></div>
<pre>&lt;RESPONSE&gt;
    &lt;STATUS&gt;Success&lt;/STATUS&gt;
    &lt;EMAILIDS&gt;30011,30234,30634&lt;/EMAILIDS&gt;
&lt;/RESPONSE&gt;</pre>
<div><strong>Response Example: Failure</strong></div>
<pre>&lt;RESPONSE&gt;
    &lt;STATUS&gt;Failure&lt;/STATUS&gt;
    &lt;ERRORCODE&gt;E400&lt;/ERRORCODE&gt;
    &lt;ERRORINFO&gt;No Email Templates were created in this account&lt;/ERRORINFO&gt;
&lt;/RESPONSE&gt;</pre>
