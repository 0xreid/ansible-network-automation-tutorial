# Configuration Generation Tutorial

This directory is meant to act as a workspace for the configuration generation tutorial. Please use this directory to follow along with the tutorial, creating your own directories and files. There are some important reference materials below for the templating and IP address calculation portion of the tutorial.

##Jinja2 formatting
For more details on Jinja2 formatting, see their [website](http://jinja.pocoo.org/docs/dev/templates/).

```
{% statements, such as for or if %}
{{ expressions to print to output, such as vars }}
{# comments #}
```

You can reference variables in two different ways. For example, the following lines do the same thing:

```
{{ foo.bar }}
{{ foo['bar'] }}
```

###If example
Use it to test a variable (presence, content, etc.).

```
{% if nanog.montreal %}
    Welcome to NANOG65!
{% elif ripe.bucharest %}
    Welcome to RIPE71!
{% else %}
    I'm not sure where I am right now...
{% endif %}
```

###For example
Loop over each item in a sequence.

```
{% for x in past-conferences %}
Name: {{ x.conf }}
Where: {{ x.city }}, {{ x.country }}
When: {{ x.date }}
# of Attendees: {{ x.attendees }}
{% endfor %}
```

###ipaddr filter

IPv4 example:
```
{{ item.ipv4 | ipv4('address') }}
{{ item.ipv4 | ipv4('network') }}
{{ item.ipv4 | ipv4('netmask') }}
{{ item.ipv4 | ipv4('broadcast') }}
```

IPv6 example:
```
{{ item.ipv6 | ipv6('host/prefix') }}
```
