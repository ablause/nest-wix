# nest-wix

Nest-wix is a javascript library with nestjs to create Wix applications.

## Installation

```bash
npm install nest-wix
yarn add nest-wix
```

## Usage

```typescript
import { Module } from '@nestjs-common';
import { EventEmitterModule } from '@nestjs/event-emitter';
import { WixModule } from 'nest-wix';

@Module({
  imports: [
    EventEmitterModule.forRoot(),
    WixModule.forRoot({
      baseUrl: 'host_url',
      appId: 'my_app_id',
      appSecretKey: 'my_secret_key',
      appPublicKey: 'my_public_key',
    }),
  ],
})
export class AppModule {}
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)