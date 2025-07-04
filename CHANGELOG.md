# Changelog

## [V6.0.0]

The kit has been fully reworked, and several objects now work differently.

* New client objects:
[Attachers](https://etohgame.github.io/kit/docs/client-objects/attachers),
[Gradient Parts](https://etohgame.github.io/kit/docs/client-objects/gradient-parts),
[GUI Displayers](https://etohgame.github.io/kit/docs/client-objects/gui-displayers), <!-- change link later -->
[Jump Launchers](https://etohgame.github.io/kit/docs/client-objects/jump-launchers),
[One-Way Platforms](https://etohgame.github.io/kit/docs/client-objects/one-way-platforms),
[Property Changers](https://etohgame.github.io/kit/docs/client-objects/property-changers),
[Swings](https://etohgame.github.io/kit/docs/client-objects/swings),
and [Sequencers](https://etohgame.github.io/kit/docs/client-objects/sequencers)
* Various additions and changes to existing client objects
* Value objects inside Client Objects have been removed in favor of `Configuration` objects for settings and [Tags](https://etohgame.github.io/kit/docs/misc#object-tags) for object flags. `ClientObject` values are also no longer needed or used.
* [Distance Culling](https://etohgame.github.io/kit/docs/client-objects/distance-culling) is now enabled by default for most physics objects to increase performance.
* There is now a [`KitSettings`](https://etohgame.github.io/kit/docs/misc#kit-settings) module found in `ReplicatedStorage` that allows you to toggle global kit settings.

A guide on converting towers made using v5.5 to v6 will be written at a later date.
