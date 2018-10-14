The transition-property property is used to specify the names of the properties that you want to apply a transition to.

You can specify either one property name, a list of comma-separated property names, or use the keyword all to indicate that all properties on an element are to be transitioned. If you don’t want any transition to be applied to any of the element’s properties, you can provide the keyword none.

When you provide a list of comma-separated property names, this list is usually mapped to a list of values provided by other transition-related properties, namely the transition-delay, transition-timing-function, and transition-duration properties. Each list of values in these properties is treated kind of like an array, where each value in a list of values has its own index. Then, each value in a list of values is mapped to its corresponding value with the same index in the list provided in the other properties.

So, when you provide a list of comma-separated property names, if the list contains properties that are not recognized by the browser or that are not animatable (transitionable), these properties must be kept in the list to preserve the matching of indices.

If a property is specified multiple times in the value of transition-property (either on its own, via a shorthand that contains it, or via the all value), then the transition that starts uses the duration, delay, and timing function at the index corresponding to the last item in the value of transition-property that calls for animating that property.

It is usually more convenient to specify the transition-property value in the transition shorthand property.

Not all properties in CSS can be transitioned. The W3C has a list of animatable types and properties in the CSS Transitions Module. Oli Studholme has also created a list of animatable CSS properties on his website that you can check out.

