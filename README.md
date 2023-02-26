# Hotel mangement API

An API powered by Express and MongoDB that stores and manages hotel rooms.

## Get Started

Clone or download this repository.

Run `yarn` or `yarn install` to install dependencies.

Run `yarn build` to build for production.

Run `yarn dev` to run in development mode.

## Technologies Used

- Node js
- Express
- Typescript
- Mongoose
- Joi
- Bcrypt
- Jsonweboken

## Create .env in src folder and paste code below

```
PORT=5000 
MONGO_URI=mongodb+srv://morahc:coldkill@cluster0.bbiy2.mongodb.net/hotel?retryWrites=true&w=majority
JWT_SECRET=Secret
```

## Endpoints

### Room

- GET `/api/v1/rooms`
- GET `/api/v1/rooms/:id`
- POST `/api/v1/rooms`  [Auth required]
- PATCH `/api/v1/rooms/:id` [Auth required]
- DELETE `/api/v1/rooms/:id` [Auth required]

### Room-types

- GET `/api/v1/rooms-types`
- POST `/api/v1/rooms-types` [Auth requied]

## Data Schema

### Room

- name `string`
- roomType `roomType`
- price `number`

### RoomType

- name `string`