# Notes:
## Flex vs Grid
- Flex understands 1D
- Grid understands 2 -> Grid will help you size the columns the same -> can also do an overlap
- Learn responsifulness
- CSS -> classes take priority
- Priority: (!important (UN)> inlline (president) > id (mother)) > class (father) > element (you)
- The ones prefered are class and element
- Not recommended to use:  (!important (UN)> inlline (president) > id (mother)) -> These cannot be overwritten

## Responsiveness
- The ability for a webpage to adjest to differet platform sizes.
- Breakpoint -> The point where the layout changes drastickly. 
- You break it when cramping of elements happens.
- With RAM you cab't control how many columns you want when breakpoint is reached.
- grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    - Tries to give all the columns 200px, if there isn't enough space for 200px min it creates a row (less columns)
    - fr -> fractional unit
- 