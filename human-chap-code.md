# Let's generate some code

Now that you are familiar with prompt engineering and how to reverse it reverse, let's earch in [blackboxai](https://www.useblackbox.io/search) how to generate typeorm definition

So I have just asked : typeorm code generation

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
