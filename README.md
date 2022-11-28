# Development

### Link to Deployed Website
https://corrosivechicken747.github.io/development/

### Goal and Value of the Application
This application can be used to visualize (or rather, fully understand the scale of) wealth inequality in the United States. Its goal is to bring perspective to how the federal minimum wage is too little, while the amount of money that Musk and other billionares make is too much.

### Usability Principles Considered
I provided the amount of time required at minimum wage to earn the money for everything in the cart. This is a good way for people to visualize the scale of how unequal wealth is. I also allow multiple copies of items in the cart, with the remove button only removing a single item. This allows for people to simulate their expenses (i.e. 4 grocery runs).

### Organization of Components
The cart and selection area are different components, and within these there is a ItemCard component for each item inside the selection area, and a CartItem for each item in the cart.

### How Data is Passed Down Through Components
Data is passed through props, with functions such as `add_to_cart` or `remove_self` implementing good separation of duties: a component is never allowed full access to the cart.

### How the User Triggers State Changes
The user triggers changes by adding or removing items from the cart. These are updated by code in a `useEffect` block.
