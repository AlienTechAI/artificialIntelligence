Hello! So here, I am going to give you some introduction about, well, neural networking. 

## Disclaimer! These notes are provided by Brilliant.org. Definitely check them out!

### Introduction to the human brain and neural networking!
The brain contains more than 808080 billion cells — called neurons — which exchange information with one another via small pulses of electricity.

![Course-Introduction-to-Neural-Networks-Re-illustration_quiz4-brain-and-neuron_3611-63_ewmnuy](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/c1a924ee-8240-4997-aadb-974188fa0c54)

One neuron doesn't talk directly with all 808080 billion others. Rather, they are connected into structures that perform specialized functions. These structures are biological neural networks.

The human brain is too complex to discuss in much detail here, but we don't need to know all the details to land on its most important characteristic — “Brains learn from experience.”

Each time you learn a new game, a dance, or a mathematical skill, neurons in your brain strengthen their lines of communication with some neurons and prune their connections to others.

The structure of a neural network evolves as you gain new abilities.

### Artificial Neurons

Just as biological neurons are the basic units of the brain, artificial neurons are the computational building blocks of an artificial neural network (ANN).

And, like biological neurons, artificial neurons respond to the information that's presented to them.

They can use this information to make predictions. 

### Layered Networks

//Refer to the chapter on Brilliant.org for in-depth knowledge

So far, we've seen a few small ANNs that make predictions about whether one cat or another is happy.

But how do we make ANNs that do more complex tasks — like predict the prices of stocks or recognize faces in photos? After all, that's what you came here for, right?

ANNs with a single neuron — like the ones we've seen so far — have limited predictive power. However, things start to get more interesting when you add more neurons.

### Seeing Digits

A few principles have emerged from our exploration with cats:

    ANNs make predictions based on their inputs.

    Neurons follow rules mechanically to compute their outputs.

By stacking neurons in layers, we create the potential to make increasingly complex predictions — as long as we can find the right connections between the layers.

The complexity of an ANN's predictions increases with the number of connections.

Just because an artificial neural network can learn doesn't mean that it thinks. 

### Computer Vision

Here's a picture that you might present to an ANN trained to perform image recognition:

![image](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/21e9a50e-25b2-45a4-a07c-5e190bfc8818)

What do you see in this picture? Deer? Bushes? A car on a driveway? 

Yes, there are deer. Four, to be precise.

In this scene, you can recognize a bunch of things — several deer, a car, leafy bushes, and grass.

The deer and bushes are similar shades of gray, but your brain can tell they aren’t the same thing. 

Your brain may even give you a sense of what the grass and flowers smell like while you stare at the scene.

Evidently, your brain is doing some significant processing. 

Identifying objects in an image is so effortless for you that you might wonder, “What’s so difficult about enabling computers to see?”

The problem is a computer has none of the built-in mechanisms that evolution has hardwired into your brain. In fact, it’s not clear what it means for a computer to see at all.

One of the things we’ll have to get used to is that computers can only think in numbers. Whether it’s a photograph, a song, or the Iliad, to the computer they’re all represented by lists of numbers. 

A digital image is represented by an array of numbers, called pixels.

Saved in a computer's memory, the scene above looks more like this — except with several thousand times as many numbers…

![image](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/efe42f94-b96f-4c0c-9a23-4cce40612ea5)

…a sight less scenic. 

### Human Vision: Context Matters

Let's begin to appreciate how difficult the problem of computer vision is by uncovering some features of the vision algorithms that run on your own personal processor — your brain.

To start, here's a small region of a photograph that we've blown up (~ 1% of its pixels). Using nothing but your biological visual system, do your best to identify what’s in this snippet of the photograph:

![image](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/28d35d26-5296-4511-8490-f96e758c341c)

A book? A plant? A chair? 

Without color, this task is a little too tough. After all, most image files on a computer store color information.

So, here’s the snippet in all its color-pixel glory:

![image](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/b742cf74-877f-4f23-826a-b791e8984d84)

What do you think it is?

A mushroom growing out of a patch of dirt? Two matches held in a cross over a table? A smokestick held against the sky? Or a car driving on a bridge?

With so few pixels, the picture is open to interpretation. You may have noticed that as you read the suggested answers, you could see fragments of truth in each description. 

When it comes down to it, the only sure way to know what the picture is depicting is to get more pixels.

Here's the full picture — a photo of the Golden Gate Bridge:

![image](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/e5f8c7eb-8915-4f7c-848e-fe42172d3654)

Wow, you put some serious time into this.

Here’s the part that the snippet is from:

![image](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/ae59dcae-b7d8-4a8b-8fb1-4ffa44122ded)

Even if you got it right, you might be surprised at how different the same set of pixels looks now that you can clearly see that the snippet is a car driving across a bridge.

With the full image, your vision system is clued in by the context of the scene to realize that the little patches are most likely cars.

When your vision system is presented with limited information, it automatically fills in details for you.

That's one of the skills a few hundred million years of mammalian evolution bought you. You're welcome.

### Human Vision: Optical Illusions

Had the patch of pixels that turned out to be a car been placed in an image of the reflecting surface of a lake, you may have interpreted the patch as a wispy cloud.

If it had been placed in an image of a nebula in deep space, you may have interpreted it as a patch of stars.

Your brain does more than matching visual information to some internal visual dictionary. Every image you see is intermingled with your previous experiences of seeing. 

Your visual system even alters your perception of abstract shapes and colors. We can learn more about these internal processes by studying optical illusions.

Here's an example. There are two gray circles separated by some distance:

![image](https://github.com/captLinuxYT/artificialIntelligence/assets/132283907/954a09c3-7e60-4bad-8a8c-33cee5e2560a)

Which circle is shaded darker gray?

The left circle? The right circle? Or are they both the same shade?

Are you sure? Look again.

To most people, the circle on the right appears significantly darker than the one on the left. It may even look like the circle on the left and the background on the right have the same color.

This illusion underscores the idea that your biological vision system is doing things behind the scenes to generate your sense of perception.

Evidently, the brain is fine with introducing some distortions in rendering the contrast between each circle and its “environment” — the different background colors.

Equally impressive are the things that the vision system chooses to simplify or transform.

Most people experience two phases of transformation. First, the empty spot will appear to turn neon green. A few seconds after that, the pink spots will disappear entirely so that it looks like only a green spot is traveling around the circle.

With all the processing that goes on in the human visual system, it's hard to know where to even begin engineering a computer vision system.

However, the past several decades have seen computer vision grow by leaps and bounds. We'll look at some of the basic ideas here, and we'll examine the architecture of the ANN that underpin the technology later in the course.

### Thinking in Pixels

Now that we have a sense of the head start we have from our vision system when identifying an object, let’s consider some basic approaches a computer vision system could use to achieve the same goal. 
