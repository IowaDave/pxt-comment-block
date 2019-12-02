# pxt-comment-block
<h3>Provides a custom block that displays user comments<br>
in-between other MakeCode programming blocks.</h3>

It is a good practice to include comments that explain what your code is doing, for two reasons:
1. Clear comments can make the code easier for someone else to read and to understand.
2. Accurate comments can make the code easier for the programmer to maintain in the future.

#### How To Use It
Import this repo as an extension to the MakeCode editor. A "Comment" group will appear amongst the main list of blocks groups, wearing a dark orange color.

Inside the group is a single block, named "comment". Drag this block to the place in your code where you want to display a comment. Replace the sample text with your actual comment.

The comment blocks are separate from other MakeCode blocks. This is different from the kinds of comments that can be embedded, that is, hidden inside regular code blocks. Embedded comments are discussed in a later section, below.

#### How The Comment Blocks Affect Your Code
The comment blocks will not cause any change in how your code works because the comment blocks do not contain any executable code instructions.

The comment blocks *do take up space* in the code that gets uploaded into the micro:bit. Relax. There is considerable capacity for both code and comments in the device's 256K of flash memory. A moderate-sized project having a few hundred blocks should still have plenty of room for comment blocks to aid understanding and future maintenance.

#### Other Ways To Embed Comments in Blocks
MakeCode also allows you to include regular JavaScript comments in your code. JavaScript comments do not take up space in the flash memory of the micro:bit, and have no effect on how your code works. 

The main difference between using a visible comment block rather than a JavaScript comment is visibility. Comment blocks are designed to display prominently in the Blocks view of the MakeCode editor.

By contrast, JavaScript comments are usually hidden from view in the Blocks side of the MakeCode editor. However, they are accessible. 

Regular blocks that contain an embedded JavaScript comment exhibit a small icon in the upper-left corner. The icon looks like a cartoon 'speech' balloon. Clicking the speech-balloon icon of a block opens a small text box to reveal the comment.
* The comment can be edited.
* The box can be resized by dragging an edge.
* The box can be closed by clicking the triangle icon. 
* The comment can be deleted by clicking the trash can icon.

There are two ways to embed a JavaScript comment inside a regular MakeCode block.
1. In blocks mode: right-click on a block, then select 'Add Comment' from the drop-down menu that appears.
2. In JavaScript mode: type the comment on the line or lines preceding the instruction that corresponds to the block.

The following code segment presents an example of the second approach:
```javascript
// A loop to display digits 0 through 9 on the
// micro:bit
loops.forLoop(0, 9, function (index) {
    basic.showNumber(index)
})
```
## TODO

- [x] Add a reference for your blocks here
- [x] Add "icon.png" image (300x200) in the root folder
- [x] Add "- beta" to the GitHub project description if you are still iterating it.
- [x] Turn on your automated build on https://travis-ci.org
- [x] Use "pxt bump" to create a tagged release on GitHub
- [x] On GitHub, create a new file named LICENSE. Select the MIT License template.
- [ ] Get your package reviewed and approved https://makecode.microbit.org/extensions/approval

Read more at https://makecode.microbit.org/extensions

## Supported targets

* for PXT/microbit
(The metadata above is needed for package search.)

