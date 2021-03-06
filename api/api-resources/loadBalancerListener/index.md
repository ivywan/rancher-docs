---
title: API
layout: rancher-default
---

## loadBalancerListener

Collection Test Description

​
### Resource Fields

Field | Type | Create | Update | Default | Notes
---|---|---|---|---|---
algorithm | enum | Optional | - | roundrobin | 
description | string | Optional | Yes | - | 
id | int | - | - | - | The unique identifier for the loadBalancerListener
name | string | Optional | Yes | - | 
privatePort | int | Optional | - | - | The private port
serviceId | [service]({{site.baseurl}}/rancher/api/api-resources/service/) | - | - | - | The unique identifier of the associated service
sourcePort | int | Optional | - | - | 
sourceProtocol | enum | Yes | - | - | 
targetPort | int | - | - | - | 
targetProtocol | enum | - | - | - | 

<br>
Please read more about the [common resource fields]({{site.baseurl}}/rancher/api/common/). 
These fields are read only and applicable to almost every resource. We have segregated them from the list above.
​

### Operations



<span class="action">
<span class="header">
Create
<span class="headerright">POST:  <code>/v1/loadBalancerListener</code></span>
</span>
<div class="action-contents">
{% highlight json %} 
{

	"algorithm": "roundrobin",

	"description": "string",

	"name": "string",

	"privatePort": 0,

	"sourcePort": 0,

	"sourceProtocol": "enum"

} 
{% endhighlight %}
</div>
</span>













<span class="action">
<span class="header">
Update
<span class="headerright">PUT:  <code>${links.self}</code></span>
</span>
<div class="action-contents">
{% highlight json %} 
{

	"description": "string",

	"name": "string"

} 
{% endhighlight %}
</div>
</span>







<span class="action">
<span class="header">
Delete
<span class="headerright">DELETE:  <code>${links.self}</code></span>
</span>
<div class="action-contents">
{% highlight json %} 
 
{% endhighlight %}
</div>
</span>






​
### Actions

<span class="action">
<span class="header">
remove
<span class="headerright">POST:  <code>${actions.remove}</code></span>
</span>
<div class="action-contents">
To remove the loadBalancerListener
<br>

<span class="input">
<strong>Input:</strong>This action has no inputs
<br>

<br>
</span>

<span class="output"><strong>Output:</strong> An updated copy of the <a href="/rancher/api/api-resources/loadBalancerListener/">loadBalancerListener</a> resource
</span>
</div>
</span>
</span>
</span>

