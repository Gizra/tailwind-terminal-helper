# Tailwind Terminal Helper

This script helps to identify which [TailwindCss](https://tailwindcss.com)
class you can use to meet a specific unit in px or rem.

You can also know which CSS rule is applied based on the class name.

# Examples

Get a class name based on a rem, px or percentage.

```
./tw width 16px
w-4

./tw width 1.5rem
w-6

./tw width 25%
w-1/4
w-3/12

./tw font-size 3rem
text-5xl

./tw text-indent 12px
indent-3
```

Get the CSS properties that are applied for a given TailwindCSS class.

```
./tw w-4
w-4     width: 1rem; /* 16px */

./tw text-sm
text-sm font-size: 0.875rem; /* 14px */
```

# Dependencies

- grep
- awk
