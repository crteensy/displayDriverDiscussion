displayDriverDiscussion
=======================

We're discussing a framework for display drivers in microcontroller applications.

__Feel free to use the wiki!__ The wiki might be useful for demonstrating certain aspects of the backend, for example.

If something needs to be added or changed, let's open an issue first to have a thread where we can track pros and cons.

Aspects we need to consider:
- [Drawing Primitives](/DrawingPrimitives.md/)
- Different [Color Spaces](/ColorSpaces.md/) (app, canvas, display)
- [Coordinate Systems](/CoordinateSystems.md/) (canvas, physical, display)
- [The Backend](/Backend.md/)
- [Display Capabilities](/DisplayCapabilities.md/)
- [Display Properties](/DisplayProperties.md/)
- and finally what [License](/WhichLicense.md/) we want to use for a possible implementation

Maybe we should also take virtual displays (one canvas that stretches over one or more displays) and cloned displays (same info on multiple displays) into account
