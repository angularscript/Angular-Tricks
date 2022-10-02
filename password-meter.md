Show the strength of an input password in red/yellow/green format.

### Install the package

```npm i ngx-password-strength-meter```

```
import { NgxPasswordStrengthMeterModule } from 'ngx-password-strength-meter';
@NgModule({
  declarations: [AppComponent, ...],
  imports: [NgxPasswordStrengthMeterModule, ...],
  bootstrap: [AppComponent]
})
export class AppModule {
  ...
}
```
### Add the password meter component to the App

```<ngx-password-strength-meter [password]="password"></ngx-password-strength-meter>```

### Configure the password strength
```
@Input() password: string;
@Input() min = 6;
@Input() max = 16;
@Input() enableLengthRule = true;
@Input() enableFeedback = true;
@Input() colors: string[] = [];
@Output() strengthChange = new EventEmitter<number>();
```
