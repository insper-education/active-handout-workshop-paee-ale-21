# Creating a new active

!!! info
    This script was created based on an example lab: **Direct Current Motor and Generator**. If you have separated a material, it is time to use it, if not, you can use the base laboratory provided.
    
    You can download the [material here](DcMotorLab.zip)

Lets create a new laboratory active on our course page, this will be done with the fallowing steps:

1. Create the laboratory folder (`02-DCMotor`) and `index.md` file
1. Add the new page to the `mkdocs.yml`
1. Add content to the active page (editing the `index.md` file)

This new content will appear on the outline of the site.

![](newlab.png){width=500}

## Creating the lab files

The way we suggest to organize the course material is:

- Each lab is a folder in `labs`
    - We suggest to enumerate the lab (`ie: 01-ExampleLab`)
- The folder will hold:
    - `index.md`: A markdown file with the class material
    - Images, presentation and extra material for the specific class
    
We will create via the github site a folder called `02-DcMotor` inside the `lab` directory and a `index.md` file on it:

- `content/labs/02-DcMotor/index.md`

Don't care about the contents of the file, let's start it with just the head:

```
# DC Motor Lab


                 .
```

!!! video
    ![](creatingLabFile.mp4)

!!! progress
    Continue

## Add the new page to the `mkdocs.yml`

Now we need to tell the mkdocs of the new page, using the same method of editing a file on the github, open the `mkdocs.yml` located at the root of your repository.

We will edit the **nav** section of this yml file adding the recent create `index.md` to the laboratories section of our page. 

```diff
nav:
  - Home: index.md
  - Classes:
    - classes/01-ExampleClass/index.md
  - Laboratories:
    - labs/01-ExampleLab/index.md
+   - labs/02-DcMotor/index.md
```

!!! video 
    ![](mkdocs.mp4)

After the build and deploy process you should see the new page on the page of your website:

![](dcMotorPage.png)

!!! warning
    Remember that the process can take up to one minute.

!!! tip
    The steps done earlier may seem complex, but once you get the hang of it, it's automatic. Local editing on your computer without using github as the editing interface is even faster and easier.

!!! progress
    Continue
    
## Adding content

**Now we come to the most interesting part of the tutorial: creating the activity that will be shared with the students.** 

For you to practice we created a fake physics lab script, made from examples provided by the discipline professors. We were not very interested in the content of the script, but rather how to port the script that was created in word for markdown and see it posted on the site.

!!! note
    Here you can choose to use our material or use what you have prepared.
    
First download the lab:

- [DcMotorLab.zip](DcMotorLab.zip)

Than extract it to your computer. You should see 5 files, been one the word document with the lab instruction and four images that were extracted from the document.

The lab script has the fallowing format (it is part/modification of one used on a real course):

![](dcMotorLab.png){width=400}

If we analyze the script, we can identify the following elements:

- Title
- Sections 
- Theory
- Equations
- Figures/ Questions/ Code 

Now you have the challenge of porting the lab to the `content/labs/02-DcMotor/index.md` markdown file. Each element listed above can be adapted for active handout/ markdown.

!!! example ""
    **TASK: Port the word lab to index.md and analyze the generated site**

!!! tip
    We suggest that you check the generated site frequently to see if it is in accordance with what you want.

!!! info 
    Markdown is practical, but it has limitations and as we use it we will learn to work around.  For ideas see:
    
    - [Basic text editing with markdown](https://insper-education.github.io/active-handout/reference/basic-editing/)
    - [Markdown extensions](https://insper-education.github.io/active-handout/reference/advanced-editing/)
    
!!! tip "Uploading image"
    You should upload the images to the lab folder before using. This can been done by the github interface:
    
    !!! video
        ![](uploadImgs.mp4)

!!! tip "You should get something like"
    ![](result.png)
