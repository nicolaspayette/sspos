## What is it?

The purpose of this model is to show how NetLogo and some of its extensions can be used to create a very simple model of the social processes of science. (This is a demo of the tools, not a claim about how science *really* works.)

To get the model, you can either clone this repository or directly download the model file:
https://raw.githubusercontent.com/nicolaspayette/sspos/master/sspos-demo.nlogo

You can then open it in NetLogo (which is available [here](http://ccl.northwestern.edu/netlogo/).)

## How it works

Choose a population size, a landscape and a network generator, and then click **setup**. A network of scientists will be created and the patches will turn into an "epistemic landscape", where higher (i.e., lighter green) positions represent more desirable ideas/hypothesis/theories/etc. The highest peaks in the landscapes are represented by red patches.

Once you press **go**, the scientists will move slightly towards one of their network neighbors, picked at random. The probability of picking each neighbor being weighted by the value of the patch that it is on: neighbors higher in the epistemic landscape have a better change of being picked.

In the case where a scientist is isolated from the rest of the network, it will just pick the patch around it with the highest value and move there.

The simulation stops when all scientists are standing on red patches. Sometimes it happens quickly, sometimes not. Different shapes of networks work best on different landscapes. You can use the BehaviorSpace tool to find out which.

## NetLogo features

To run this model, you need:

- The [Landscapes Extension](https://github.com/NetLogo/Landscapes-Extension#netlogo-landscapes-extension) for generating the epistemic landscape;

- The [NW extension](https://github.com/NetLogo/NW-Extension#the-netlogo-nw-extension-for-network-analysis) to generate the epistemic network;

- And the [Rnd extension](https://github.com/NetLogo/Rnd-Extension#netlogo-rnd-extension) for weighted random selection.

## Credits

Authored by Nicolas Payette for demo at the [Simulating the Social Processes of Science workshop](http://www.lorentzcenter.nl/lc/web/2014/607/info.php3?wsid=607&venue=Oort), Leiden, NL, April 2014.
