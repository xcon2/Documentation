<!-- TITLE AND DEFINITION starts -->

{% assign title = "Trigger-On Event" %}
{% assign definition = site.data.trading_system.trigger-on_event %}
{% assign preposition = "the" %}

<!-- TITLE AND DEFINITION ends -->

{% if include.heading != "" %}
{{include.heading}} {{title}}
{% endif %}

{% if include.icon != "no" %} 

{% if include.table == "y" %}
<table class="definitionTable"><tr><td>
{% endif %}

<img src='images/icons/{{include.icon}}{{ title | downcase | replace: " ", "-" }}.png' />

{% if include.table == "y" %}
</td><td>
{% endif %}

{% endif %}

{% if include.definition != "regular" %}

<strong>{{ definition }}</strong>

{% else %}

{{ definition }}

{% endif %}

{% if include.table == "y" and include.icon != "no" %}
</td></tr></table>
{% endif %}

{% if include.content != "n" %}

<!-- CONTENT starts -->

In conceptual terms, the trigger-on event is the mechanism you use to define the specific situations in which you would consider trading with the corresponding strategy. Think of the trigger-on event as the definition of the scenario in which the trading idea behind the strategy should be carefully considered.

Once a strategy is triggered-on, the system starts evaluating the take position event. In conceptual terms, it means that the system has been alerted that the trading idea behind the corresponding trading strategy has produced a signal and that it should carefully monitor the market for the opportunity to take a position.

<!-- CONTENT ends -->

{% endif %}

{% if include.adding != "" %}

{{include.adding}} Adding {{preposition}} {{title}}

<!-- ADDING starts -->

To add a trigger-on event node, select *Add Missing Events* on the trigger stage node menu. All events that may be missing are created along with the rest of the basic structure of nodes required to define each of them.

<!-- ADDING ends -->

{% endif %}

{% if include.configuring != "" %}

{{include.configuring}} Configuring the {{title}}

<!-- CONFIGURING starts -->

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

<!-- CONFIGURING ends -->

{% endif %}