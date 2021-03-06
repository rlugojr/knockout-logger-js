knockout-logger-js
==================

A logger that can be displayed on the page and/or in the console on any device.

<h1>Scenarios that this widget can be useful:</h1>
<ul>
   <li>You don't want your logs to appear in the console in production.</li> 
   <li>You want to keep the useful logging code in the code base.</li>
   <li>You don't want the logs to slow down the app (use a function as logFactory in this case).</li>
   <li>You want to see logs where they are not easy to be seen, e.g. on mobile devices.</li>
   <li>
      You want a more rich and convenient UI than the native browser console that can do the following and more:
      <ul>
         <li>Timestamping</li>
         <li>Grouping/filtering/searching</li>
         <li>Logs kept after page refresh</li>
      </ul>
   </li>
</ul>

<h1>Usage</h1> 
(assuming the variable name loaded from Require is 'Logger'):

<code>Logger.debug(logGroupName, logFactory(string|function))</code>: output a debug log.<br />
<code>Logger.log(logGroupName, logFactory(string|function))</code>: output a regular log.<br />
<code>Logger.warn(logGroupName, logFactory(string|function))</code>: output a warn log.<br />
<code>Logger.error(logGroupName, logFactory(string|function))</code>: output an error log.<br />

Turn on/off the logger on the page/in the console by adding the following query string params to the url and refreshing the page:
<code>?logger=[true|false]&console=[true|false]</code>


<h1>Dependencies:</h1>

<ul>
   <li>KnockoutJS (2.2.0+) - http://knockoutjs.com/</li>
   <li>SugarJS (1.4.0+) - http://sugarjs.com/</li>
   <li>RequireJS (2.0.0+) - http://requirejs.org/</li>
   <li>Bootstrap (3.0.0+) - http://getbootstrap.com/</li>
   <li>Storage
</ul>
