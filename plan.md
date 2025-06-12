# Project Plan: ApexHost

**Description:** A simple and affordable web hosting platform built with Ruby on Rails, focusing on ease of use and basic domain management.


## Development Goals

- [ ] Install and configure the tailwindcss-rails gem: `rails tailwindcss:install`. Then customize application.tailwind.css with basic styling and color scheme.
- [ ] Implement model validations for the Domain model: name (presence, uniqueness), plan (inclusion in a predefined list - 'basic', 'standard', 'premium').
- [ ] Customize the Domain scaffold views (index.html.erb, show.html.erb, _form.html.erb) to utilize Tailwind CSS classes for improved aesthetics and responsiveness.
- [ ] Modify the Domains controller to ensure that each domain is associated with the currently logged-in user.  Override the `create` action to assign `current_user` to the `user` attribute.
- [ ] Implement a basic user dashboard that displays a list of domains owned by the current user. This may require a new action in the Domains controller and corresponding view.
- [ ] Add a 'Welcome, [username]!' message and a list of domains to the root page (index).
- [ ] Implement a simple pricing plan display. Users can upgrade their current plan via a dummy 'upgrade' button.
- [ ] Protect domain actions using authorization.  For example, only the owner of a domain should be able to edit or delete it.
- [ ] Seed the database with a few sample users and domains for testing.
