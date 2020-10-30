# uftone-web-aos-gui-for-340

## Description
This repository is used as a resource for the UFT One level 340 training.

It shows all of the major capabilities and benefits of UFT One GUI testing using traditional attribute based object identification. It runs against public AOS, but of course you can change the URL to Nimbus AOS if desired. 

# WARNING
Because of the repository organization, to use this repository, you must execute the git switch commands as detailed below, *before* you can open the UFT tests. **Please read this file!**

## Usage

There are multiple UFT tests, with multiple branches in the repository.

The tests/branches are

1. main
2. record-replay-report
3. augmented
 
Each branch will now be discussed in a bit more detail.

## Branches

### main
There is nothing in this branch, except for the readme

### record-replay-report
#### One UFT test within this branch, "my Customer2"

**Note: in order to see this test, after cloning the repository you must run** *git switch record-replay-report*

This is a simple recording of shopping; adding an item to the cart; clearing the cart.

With AOS, it is always best to click on the word associated with a category and item, as the object is easier to identify. If you click on the pictures, a cryptic "image1234.png" gets recorded.

Change the number of items by changing the numerical quantity, as this is the only value that is easy to parameterize.

Be sure to record a checkpoint.

If not using Nimbus, be sure to enable the run-time setting to capture a screen shot on each step.

### augmented

There are two UFT test within this branch, 

**Note: in order to see these tests, after cloning the repository you must run** *git switch augmented*


#### An augmented version of the "my Customer2" test.

* In this branch, the shopping cart has been modified to use a regular expression to identify the cart, regardless of how many items were added. 
* An output has been created
* Several enhancements were added to object descriptions, including using both regular expressions and parameterized values.

#### A new test "dataDrive"

This is a totally different test, created with auto parameterization, than many values added using the TCG. Demoing creating many values is great, but in this branch, the test-settings have been set to only run a few iterations, so that playback is faster

