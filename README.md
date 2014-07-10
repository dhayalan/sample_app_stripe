# SampleApp

This is a social network for developers. It's our sample Rails
application, showing how to use Stripe to charge subscribers.

we used the Stripe Javascript bindings to validate a credit card, and
the Stripe Ruby bindings to create a customer and add the credit card to that
customer. Customers can also update their credit card.

## Installation steps

You will need a publishable token and a secret token. Add them both to
config/initializers/stripe.rb.

Create a plan with the ID "premium" on your
[account](https://manage.stripe.com/#test/plans)

Install the bundler gem if you don't already have it

Run the following commands to setup the project

    bundle
    bundle exec rake db:setup
    bundle exec rails s
