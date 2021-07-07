# Adding interactive content

Now let's see how to add interaction to the lab done previously, for that we'll use some tools developed by us and that integrate in the infrastructure used previously. The system composed of opensource tools + our extensions is called Insper Active Handout and has its own page that can be accessed at:

- https://insper-education.github.io/active-handout/

And you can track the development and the new ideas that will be implemented on the git repository:

- https://github.com/insper-education/active-handout/issues

!!! info
    If you want you can contribute to the project by giving suggestions for new tools (open a new issue), participate in the discussion of an existing issue or help with the implementation of new features/bug fixes.

==All tools are accessed via markdown commands==, it's one of our development principles, not having to rely on creating and editing on external tools. This facilitates the creation of new content and the possibility of using the versioning system in the course material

## Interactions

Now let's see some tools available for use and we'll use them to modify our previously created lab by adding interactivity to it.

### Video

!!! info ""
    Please access the [Video plugin page](https://insper-education.github.io/active-handout/reference/quiz/) for more information 

To add a video to your lab use the fallowing syntax:

```
!!! video
    ![Video title](video_src)
```

!!! info
    Can be a local video or a youtube video, the tool the tool automatically detects and adapts.
 
!!! task
    Add a video to the begin of the lab, the video can be a brief review of the subject or some content that motivates/curiosities about the lab.
 
### Quiz

!!! info ""
    Please access the [Quiz plugin page](https://insper-education.github.io/active-handout/reference/quiz/) for more information 

You can easily add a quiz using the fallowing syntax:

=== "markdown"
```
!!! question choice
    Text of the question. 

    - [ ] option 1
    - [ ] option 2
    - [X] correct option


    !!! details
        Text explaining correct answer. Only shown after option is selected.
```
    
## Task 1 - 

## Task 2 - 
