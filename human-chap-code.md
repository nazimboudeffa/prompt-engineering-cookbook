# How to write code

To write code there are multiple manners :

* From your expertise and long experience
* From your inspiration but code is code so you'll use your knowledge/datas/old code
* From Googling or tutorial on YT
* From StackOverflow

But like we've seen in the forewords, some jobs will disapear because the coders are too specialised

I am one of the big fan of copy past adapt from stackoverflow (particularily with new frameworks) but with ChatGPT it started to be better to understand new technologies

# Let's generate some code

Now that you are familiar with prompt engineering and how to reverse it, let's search in [blackboxai](https://www.useblackbox.io/search) how to generate typeorm models

So I have just asked blackboxai in the search box : typeorm code generation

It answered the following code

```
import { Entity, PrimaryGeneratedColumn, Column } from "typeorm"

@Entity()
export class User {
    @PrimaryGeneratedColumn()
    id: number

    @Column()
    firstName: string

    @Column()
    lastName: string

    @Column()
    age: number
}
```

Now let's reverse prompt engineer it on ChatGPT

```
Reverse engineer the following {code} in to a prompt

code = 
import { Entity, PrimaryGeneratedColumn, Column } from "typeorm"

@Entity()
export class User {
    @PrimaryGeneratedColumn()
    id: number

    @Column()
    firstName: string

    @Column()
    lastName: string

    @Column()
    age: number
}
```

Here is the answer of ChatGPT

Create a User entity using TypeORM that has the following properties:

* id: a unique identifier that is automatically generated
* firstName: a string that represents the user's first name
* lastName: a string that represents the user's last name
* age: a number that represents the user's age

The entity should be decorated with the @Entity() decorator, and each property should be decorated with the appropriate decorator (@PrimaryGeneratedColumn() for the id, and @Column() for the firstName, lastName, and age properties).

This is very inspiring right ?

So let's continue
