# uftone-web-aos-gui-for-340

## Description
This test is used as a resource for the UFT One level 340 training.

It shows all of the major capabilities and benefits of UFT One GUI testing using traditional attribute based object identification. It runs against public AOS, but of course you can change the URL to Nimbus AOS if desired. 

## Usage

There are 3 branches. Each branch reflects the UFT test at the end of one of the use cases presented in the 340 training. They branches are
1. record-replay-report
2. augmented
3. auto-param-and tcg
Each branch will not be discussed in a bit more detail.

## Branches

### record-replay-report
This is a simple recording of shopping; adding an item to the cart; clearing the cart.

With AOS, it is always best to click on the word associated with a category and item, as the object is easier to identify. If you click on the pictures, a cryptic "image1234.png" gets recorded.

Change the number of items by changing the numerical quantity, as this is the only value that is easy to parameterize.

Be sure to record a checkpoint.

If not using Nimbus, be sure to enable the runtime setting to capture a screen shot on each step.

### augmented

In this branch, the shopping cart has been modified to use a regular expression to identify the cart, regardless of how many items were added.

An output value was also added.

### auto-param-and tcg

This is a totally different script, created with auto parameterization, than many values added using the TCG. Demoing creating many values is great, but in this branch, the test->Settings have been set to only run a few iterations, so that playback is faster

