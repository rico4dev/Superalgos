<!-- TITLE AND DEFINITION starts -->

{% assign title = "Initial Take Profit" %}
{% assign definition = site.data.trading_system.initial_take_profit %}
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

Pretty much like with the initial stop, the initial take profit is a target, and not an order to be placed. Only when the trading bot instance detects that the target has been hit does it place an order to close the trade.

The initial target is set in phase 0, which may shift to the following phase once the corresponding next phase event is validated.

<!-- CONTENT ends -->

{% if include.adding != "" %}

{{include.adding}} Adding {{preposition}} {{title}}

<!-- ADDING starts -->

To add an initial take-profit node, select *Add Missing Items* on the initial definitions node menu. All items that may be missing are created along with the rest of the basic structure of nodes required to define each of them.

<!-- ADDING ends -->

{% endif %}

{% if include.configuring != "" %}

{{include.configuring}} Configuring the {{title}}

<!-- CONFIGURING starts -->

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

<!-- CONFIGURING ends -->

{% endif %}