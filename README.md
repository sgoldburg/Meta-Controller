# Meta-Controller

A Max patch built around MIRA objects that allows storage of and interpolation between sets of parameter states. With the MIRA app open on an iPad, the user is presented with a touch-based interface for the patch. The iPad interface allows the user to navigate between sets of parameter states in two dimensions. Interpolation "gestures" may be looped; in theory there is no limit to the length of a gesture that may be captured and looped. Parameter values are output by Max as standard MIDI CC messages, and are freely assignable from the patch interface.

The patch is easily extensible and capable of supporting a greater number of parameters, states, and interpolation dimensions in order to best suit the user's needs. As implemented, four parameter states of eight values each are arranged around the corners of a rectangular interpolation area on the iPad interface. If a user does not wish to use the iPad interface, the patch is readily programmed from the computer, and any control data input may be routed to the interpolation engine. For example, the Sensel Morph could easily be swapped in as an interpolation interface, enabling interpolation in three dimensions.

How to Use the Patch:
1. Assign the MIDI port and CC #'s to be output by the patch.
2. Store sets of parameter values as states. The toggles next to the parameter value dials control whether parameters are affected by the interpolation engine. If a user wants manual control of a specific parameter value, they may turn off the toggle next to the relevant parameter value dial.
3. Interpolate between parameter states. Gesture looping may be toggled on and off. When gesture looping is toggled off, any previously recorded gesture will remain in memory and will resume when gesture looping is toggled on again. Initiating a new gesture will interrupt and replace any currently looping gesture.

Tips:
- Store distinct parameter values in each state. Interpolate between these states until you find something you like. Store the current parameter values as a new state. Rinse and repeat. When an active state is overwritten in this process, the parameter values output by the patch will adjust immediately to reflect the new space of interpolable states.
