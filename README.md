ember-cli-101-errata
====================

Errata of the Ember.js book https://leanpub.com/ember-cli-101.

## Hands-on

Where it reads:

> In our example, we are manually checking that all the fields are not
> empty by using the isEmpty47 helper.  With our naive validation in
> place, we can now modify our save and cancel actions:

It should probably clarify whether route or controller actions should be
modified.

Where it reads:

> Why? As we have said previously, Ember.js is based on convention
> over configuration. The pattern of having dynamic segments like
> model_name_id is so common that if the dynamic segment ends with
> _id, then the model hook is generated automatically by calling
> this.store(‘model_name’, params.model_name_id).

It should probably read:

> Why? As we have said previously, Ember.js is based on convention
> over configuration. The pattern of having dynamic segments like
> model_name_id is so common that if the dynamic segment ends with
> _id, then the model hook is generated automatically by calling
> this.store.find(‘model_name’, params.model_name_id).

Where it reads:

> When we pass our intended route and an instance of a friend to
> link-to, it maps the property id to the parameter user_id(we could
> also pass friend.id). Then, inside the block, we render the content of
> our link tag, which would be the first and last name of our friend.

It should probably read:

> When we pass our intended route and an instance of a friend to
> link-to, it maps the property id to the parameter friend_id (we could
> also pass friend.id). Then, inside the block, we render the content of
> our link tag, which would be the first and last name of our friend.

Where it reads:

> If we recall in /app/templates/friends/index.hbs, we never mentioned
> model and yet we got our friends listed by only adding {{#each}} and
> referencing the properties of the models.

It should probably read:

> If we recall in app/templates/friends/index.hbs, we never mentioned
> model and yet we got our friends listed by only adding {{#each}} and
> referencing the properties of the models.

Where it reads:

> 2. Add a link so we can move from app/index.hbs to the index.

It should probably read:

> 2. Add a link so we can move from app/templates/index.hbs to the
> list of friends (might need to generate the missing template).

Where it reads:

> This means that if we are in Friends Show Route or Friends Edit Route,
> we can move between them by simply referencing the route without the
> dynamic segment:

This doesn't seem to work on 1.8.1.

## PODS

Where it reads:

> Currently we can structure our projects using pods or grouping things
> by their time, but the way forward is to start using pods, Ember.js
> 2.0 will introduce the concept of Routeable Components and it will
> expect us to place some files following a pod convention.

It should probably read:

> Currently we can structure our projects using pods or grouping things
> by their type but, the way forward is to start using pods. Ember.js
> 2.0 will introduce the concept of Routeable Components and it will
> expect us to place some files following a pod convention.
