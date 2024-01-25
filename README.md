<p align="center">
  <a href="https://github.com/https://github.com/mohrazzak/better-nestjs-zod-prisma">
    <img src="/logo.svg" alt="NestJS Zod Prisma" width="120" height="120">
  </a>
  <h1>better-nestjs-zod-prisma</h1>
  <p align="center">
    ✨ This is edited nestjs-zod-prisma with new features ✨
  </p>
</p>
<br/>
</p>

## New Features

It now supports Swagger out of the box, you can just have your schema defined and it will be swaggered using the `@anatine/zod-openapi` and also you can customize that using `.openapi()`

## Improvements

`nullable` instead of `nullish` when it comes to the optional fields which make sense more.

## Bug Fixed

When it comes to Enums this package had a big issues, one of them is duplicated imports that is resolved in this enhanced package

another issue was TypeError between Enums that defined in Prisma and the generated zod schema that has enum so we fixed that to use the prisma enums to match the prisma type

and a lot more..

## Missing features

Only one missing feature which is `z.from(schema)` because we switched from using `nestjs-zod` to `@anatine/zod-openapi` but we can achieve same goal by using this way `@z.custom().and(schema)`
And I am open and happy to improve that.

## What does this package needs

This package needs editing the tests to match the changes
and also needs better Readme file
So I would be happy if someone helped me in that

## About The Project

Zod Prisma doesn't work well with `nestjs-zod-prisma` and its author has been inactive for a long time - so I created this fork to fix the problems that I suffered from.

To work better with `nestjs-zod`, this library provides a little different API for Prisma rich comments directives.

You can use `@z.custom().and(imports.schema)` for using your own schemas.

Also, this library generates DTOs for better NestJS integration. It's done using `createZodDto` from `@anatine/zod-nestjs`.

#### And it also support `.openapi` that was missing form the original package

And we still support the JSDoc comments.

## Contact

Mohammad Abdalrazzak - mhorazzak7@gmail.com
Discord - username: saybers, id: 304257501980000277

Project Link: [https://github.com/mohrazzak/better-nestjs-zod-prisma](https://github.com/mohrazzak/better-nestjs-zod-prisma)

Project Link: [https://github.com/risen228/nestjs-zod-prisma](https://github.com/risen228/nestjs-zod-prisma)
