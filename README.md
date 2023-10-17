<p align="center">
  <a href="http://nestjs.com/" target="blank">
    <img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" />
  </a>
</p>

<p align="center">
  S3 driver for Factory drive module from NestJS framework
</p>

<p align="center">
  <a href="https://www.npmjs.com/org/streamkits"><img src="https://img.shields.io/npm/v/@streamkits/nestjs_module_rcon.svg" alt="NPM Version" /></a>
  <a href="https://www.npmjs.com/org/streamkits"><img src="https://img.shields.io/npm/l/@streamkits/nestjs_module_rcon.svg" alt="Package License" /></a>
  <a href="https://github.com/StreamKITS/nestjs_module_rcon/actions/workflows/ci.yml"><img src="https://github.com/StreamKITS/nestjs_module_rcon/actions/workflows/ci.yml/badge.svg" alt="Publish Package to npmjs" /></a>
</p>
<br>

# S3 driver for Factory drive module
S3 driver for Factory drive module from NestJS framework

## Usage
```ts
@Module({
  //...
})
export class AppModule {
  public constructor(storage: FactorydriveService) {
    // If you want to add a new driver you can use the registerDriver method
    storage.registerDriver('s3', AwsS3Storage)
  }
}
```
