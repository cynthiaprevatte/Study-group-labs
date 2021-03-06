# Variables

With values and operators, the computer can do work for us.

Let’s calculate the cost of a road trip.
If we’re driving 300 miles in a car that gets 30MPG and gas costs $2.50 per gallon:

    300 / 30  #> 10 gallons of gas needed
    10 * 2.50  #> 25.0 total cost

Great!

What if our friend wants to calculate the cost of their road trip?
They have to write a totally _different_ program since the values changed.

We should write our instructions to work on _abstract_ values. Then the user can put in new inputs and the program will give them useful outputs.

You can reference abstract values in code via **variables**. They are bare words with no quotes:

    miles
    recipient_email_address
    game_is_over

A variable is just like a _labeled box_ with a value inside. You have to make up the variable name. It should represent how to _interpret_ the value inside.

Writing out our road trip calculator with abstract variables:

    miles / miles_per_gallon
    gallons_needed * cost_per_gallon_of_gas

How do we fill our abstract variables with actual values? You **assign** the result of an expression to a variable:

    miles = 30.5

Variables are free! If the meaning of a value has changed, even a little, make a new variable with a different name so you remember the different meaning.

    distance_miles = 100
    distance_feet = 5280 * distance_miles

Variables are _also_ expressions, like literals and the operators with inputs. When you **reference** a variable in an expression, out pops the _last assigned_ value.

Again, all expressions are interchangeable:

    greeting = 'Hi, ' + 'David'
    your_name = input_name
    next_number = old_number + 1

Remember, variable names are for you. The computer doesn’t understand them. It just follows instructions.

------

## Basic Naming

Variable names can only be upper case letters, lower case letters, underscores, and numbers. Numbers cannot begin a variable name.

Proper Python style has variables in `snake_case`: words are all lowercase and separated by underscores.

If a variable is effectively a constant, they are in `CONSTANT_CASE`: words are all uppercase and separated by underscores.
