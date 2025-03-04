---
title: Rides
layout: page
permalink: /rides
---
{% for ride in site.rides %}
    ## {{ ride.title }} {% if ride.category == "saturday" %} *Saturday Ride* {% endif %}
    ### {{ ride.headline }}
    ### {{ ride.date | date_to_string: "ordinal", "US"}}
    Meet-Up @ {{ ride.start}}
    & ride with us {{ ride.length }} to
    {{ ride.end_time }} @ {{ ride.end}}
    // eventually I want an image included here too
{% endfor %}

Content check


