# Zigat.com similar restaurants module
> This module shows similar restaurants to the one displayed on a page by category and neighborhood.

## Related Projects
  - https://github.com/FEC-7-Stevens/photo-carousel-service
  - https://github.com/FEC-7-Stevens/info-sidebar-service
  - https://github.com/FEC-7-Stevens/tips-recommendations-service

## Table of Contents
1. [Usage](#Usage)
2. [Requirements](#Requirements)
3. [Development](#Development)
4. [Screenshots](#Screenshots)

## Usage
> Example URL: http://localhost:3004/2/

To initialize the page, in two separate terminal windows:

```sh
npm start
npm run build
```

If there are no similar restaurants the module doesn't render. Example: http://localhost:3004/73/

## Requirements
- Node v12.18.1
  - https://nodejs.org/
- MySQL v5.7.31
  - https://dev.mysql.com/

## Development

### Installing Dependencies
From within this repository's root directory:
```sh
npm install
```

### Database Creation and Seeding
First create the schema, then add 700 restaurants data with relative photos.
```sh
npm run schema
npm run seed
```

### Development Enviroment
In two separate terminal windows:
```sh
npm run start:dev
npm run build:dev
```

### Testing
Using Jest and Enzyme.
```sh
npm test
```

## Screenshots

### Similar restaurants full grid of six
Example: http://localhost:3004/2/

![Alt ](/screenshots/similar-grid-6.png?raw=true "Similar restaurants full grid of six")

### Similar restaurants grid of four
Example: http://localhost:3004/16/

![Alt ](/screenshots/similar-grid-4.png?raw=true "Similar restaurants grid of four")

### Similar restaurants grid of two
Example: http://localhost:3004/4/

![Alt ](/screenshots/similar-grid-2.png?raw=true "Similar restaurants grid of two")

### One restaurant has no photos
Example: http://localhost:3004/4/

![Alt ](/screenshots/similar-with-exception.png?raw=true "One restaurant has no photos")
