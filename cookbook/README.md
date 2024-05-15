While the cookbook may seem pretty self-explanatory, certain values are a bit more complicated. Hence, why I'm here to help you understand them! Or, at least, attempt to - I myself do not fully understand how some of these values are calculated.

## 'Nutrition' and 'Saturation' values?

The Nutrition value is fairly simple - Setting an item's nutrition to 1 will provide half a hunger. Setting this value to 2 will provide 1 hunger, and so forth.

However, to determine the saturation value, it's a bit of a different story. You see, the saturation value is not set directly by a person - instead, it is calculated according to the saturation modifier and the nutrition value.

The saturation value is equivalent to the result of, N times M - N is the nutrition value while M is the saturation modifier. For example, setting the nutrition value to 8 and the saturation modifier to 0.4 (because, yes, this value <strong>must</strong> be a decimal value/float value) will give you the following equation: 8*0.4=3.2. This means that the saturation value for this item is 3.2. This value can easily be seen while using mods such as Appleskin, which assisted in confirming these calculations.

I tried looking for resources regarding this, but couldn't find anything. If anyone has any idea as to how this is calculated, it is very much appreciated.

## Saturation modifier?

Yes, as mentioned previously, instead of setting a static saturation value similar to nutrition, it is required to input a float value (such as 0.4F or 0.4f) inside of the proper method - .saturationMod(float saturationModifier).
