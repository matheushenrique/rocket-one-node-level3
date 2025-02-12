# APP

GymPass style app

## RFs (functions rules)

- [x] It should be possible to register;
- [x] It should be possible to authenticate;
- [x] It should be possible to obtain the profile of a logged user;
- [x] It should be possible to obtain the number of check-ins performed by the logged user;
- [x] It should be possible for the user to obtain their check-ins history;
- [x] It should be possible for the user to seek nearby gyms (up to 10km);
- [x] It should be possible for the user to seek gyms by the name;
- [x] It should be possible for the user to check in at a gym;
- [x] It should be possible to validate a user's check-in;
- [x] It should be possible to register a gym;

## RNs (business rules)

- [x] The user should not be able to register with a duplicate email;
- [x] The user cannot do 2 check-in on the same day;
- [x] The user cannot check in if not close (100m) from the gym;
- [x] Check-in can only be validated up to 20 minutes after being created;
- [ ] Check-in can only be validated by administrators;
- [ ] The gym can only be registered by administrators;

## RNFs (non-function rules)

- [x] The user password must be encrypted;
- [x] Application data need to be persisted in a postgresql bank;
- [x] All data lists need to be paid with 20 items per page;
- [ ] The user must be identified by a JWT (JSON Web Token);

## Tools and Technologies used

### Typescript
### Eslint
### Fastify
### Prisma

To auto generate migration
``` 
npx prisma migrate dev
```
To see the tables and the data in the database
```
npx prisma studio
```
### Zod
### Docker
To create docker with the image provided in docker-compose file
```
docker compose up -d
```

### Vitest


## TODO

take a look at renovate to automate process of updates
https://docs.renovatebot.com/getting-started/use-cases/