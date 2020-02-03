<!-- TITLE AND DEFINITION starts -->

{% assign title = "Trigger-Off Event" %}
{% assign definition = site.data.trading_system.trigger-off_event %}
{% assign preposition = "the" %}

<!-- TITLE AND DEFINITION ends -->

{% if include.heading != "" %}
{{include.heading}} {{title}}
{% endif %}

{% if include.icon != "no" %}
<img src='images/icons/{{include.icon}}{{ title | downcase | replace: " ", "-" }}.png' />
{% endif %}

**{{ definition }}**

<!-- CONTENT starts -->

In conceptual terms, the trigger-off event is the mechanism you use to define the situation in which the corresponding strategy should stop considering the trading opportunity signaled by the trigger-on event. That is, you use the trigger off event to describe the scenario for the invalidation of the trading idea behind the strategy.

Once a strategy is triggered-on, only two possible scenarios may follow. Either the take position event is triggered, thus, taking a position and opening a trade, or the trigger-off event is triggered first.

In the first scenario, the strategy remains *on* until the trade is closed. As the trade is closed, the strategy is triggered-off. In the second scenario, the strategy is triggered-off immediately.

<!-- CONTENT ends -->

{% if include.adding != "" %}

{{include.adding}} Adding {{preposition}} {{title}}

<!-- ADDING starts -->

To add a trigger-off event node, select *Add Missing Events* on the trigger stage node menu. All events that may be missing are created along with the rest of the basic structure of nodes required to define each of them.

<!-- ADDING ends -->

{% endif %}

{% if include.configuring != "" %}

{{include.configuring}} Configuring the {{title}}

<!-- CONFIGURING starts -->

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

<!-- CONFIGURING ends -->

{% endif %}