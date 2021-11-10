#Blitz RealWorld

[React](https://reactjs.org) + [NextJS](https://nextjs.org) + [Prisma](https://www.prisma.io)

A FullStack [RealWorld Starter App](https://codebase.show/projects/realworld?category=fullstack)

##Set Up Your Computer

You need Node.js 12 or newer. You can verify this by running `node -v` in your terminal. If you don't have Node or need a newer version, we recommend using a node version manager like [fnm](https://github.com/Schniz/fnm) so you can change node versions for each project.

##Install Blitz

Run `yarn global add blitz`

##Create a New App

`blitz new myAppName`
`cd myAppName`
`blitz dev`  

View your brand new app at [http://localhost:3000](http://localhost:3000)


##Add RealWorld model to your app

To create a RealWorld 2.0 site, copy schema.prisma into the db folder to provide:

RealWorld tables: User, Article, Content, Tag
Blitz tables: Session, Token, Project, Question, Choice
Neighborhood tables: Org, Event, Service, Item

To run only the simple RealWorld 1.0 schema, copy realworld.prisma to db/schema.prisma.

Generate the model by running:
`blitz generate all project name:string`
Select Yes to run the Prisma migrate
Choose a name, then restart the server

`Ctrl + c`
`blitz dev`

Then go to [http://localhost:3000/projects](http://localhost:3000/projects)