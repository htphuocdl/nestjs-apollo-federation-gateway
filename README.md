# nestjs-with-apollo-federation-gateway
![PlantUML model](https://www.plantuml.com/plantuml/dsvg/ZP9FImCn4CNl-HJ3tli5HAH5YnIKeblfeNWOatGtc4sMIIB-eT_TsXLt0cj93Wl3cz--zs3c8IB5r5aXfFL9mPU0uziJTXggbOkQ75e8cjwCrA4QzDFRtM1eNpoIWdgGdqTjJGqwyudHU3SXBr9iFPtHfVJ9nLmvdBxY7s-udCskZcJlhVLmkmNp6tw0yqIbK9wJKzCG3rzYKbn6lvUNuL1v6GwLb-7xX_o6TflMa88UANxyY5FCOCuNB-1nMM_soHRlDuHz-t0dH8_o5HiDrT8fU0gQ_iuLPVG4s_jhDgtMDPiMJf4tAezf7BFblnrDvzgfrDbl)

# Quick start
## Deploy
```
docker-compose up -d
```
- [Apollo Gateway](http://localhost:3816/graphql)
- [Auth Service](http://localhost:3817/graphql)
- [Home Gateway](http://localhost:3818/graphql)
## Develop
```
docker-compose -f docker-compose-dev.yml --env-file .env.example up -d
```
- [Apollo Gateway](http://localhost:3816/graphql)
- [Auth Service](http://localhost:3817/graphql)
- [Home Gateway](http://localhost:3818/graphql)
# Detail
