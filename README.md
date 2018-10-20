# What is this?

Snippets cheat sheet that I am putting together to help anyone that needs to learn important coding topic or just use it as a refresher :boom: :raised_hands:

enjoy!


# Table of content:

- [JavaScript](#javascript)
    - [Classes](#classes)
    - [Promises](#Promises)
    - [Await/Async](#await/async)
- [Angular](#angular)
    - [Angular CLI](#angular-cli)
    - [Modules](#Modules)
    - [Routes](#routes)
    - [Components](#Components)
    - [Directives](#Directives)
    - [Services](#Services)
    - [Pipes](#Services)
    - [Observables](#Observables)
- [TypeScript](#typescript)



## Javascript

- [ ] What is JavaScript ?

### Classes 

- [ ] JavaScript Class ?

```

class Tesla{

constructor(){


}



}

```


### Map function 

```
const cars = [
  { name:'BMW', id:1 },
  { name:'Tesla', id:2 },
  { name:'Audi', id:3 }
];
```
```
const carNames = cars.map(car => car.name);
console.log(carNames); //["BMW", "Tesla", "Audi"]
```

### Filter

```
const electricCar = carNames.filter(car => car !== "Tesla")
console.log(electricCar)//["BMW", "Audi"]
```

### For in loop

```
let array = [1,2,3];

for ( let i in array){
  
  console.log(array[i]);
  
}
```

### Promises

Callbacks alternatives

```
function delay(ms) {
  return new Promise(resolve => setTimeout( resolve, ms));
}
```

```
delay(3000).then(() => alert('runs after 3 seconds'));
```

### Await/Async

Promises alternative

```
const asyncRequest = async () => {

    const val1 = await promise(val1)
    const val1 = await promise(val1)
    return promise(request1, request2)

}

```




## Angular

- [ ] What is Angular ?
- [ ] Angular CLI ?

## Angular CLI

Angular Command line, helps automate some process like generating and building out app

### Routes
Sample routes snippet
```
const routes: Routes = [
  { path: '', loadChildren: './tabs/tabs.module#TabsPageModule' },
  { path: '**', loadChildren: './tabs/tabs.module#TabsPageModule' }

];
```
### Modules

### Components

### Directives

### Built Directives

```
*ngIf="(users$ | async).length"
*ngFor="(let user of users$ | async)"

```
### Services

- [ ] What are services used for?
 
### Pipes

- [ ] Async pipes
- [ ] Subscribe to an Observable
  
### Observables
- [ ] What is Observables
- [ ] Create Observable

Import Observable and HttpClient

```
import { Observable } from 'rxjs';
import { HttpClient } from '@angular/common/http';

```
Get http API resources

```
public posts$ :Observable<any>

constructor(public http:HttpClient){}

ngOnInit() {

    this.posts$ = this.getPosts();

}

getPosts(): Observable<any[]> {

    return this.get.http<any[]>('ENTER_API_URI', {
        params: {
          per_page: '12'
        }
      });
}


```


```
Subscribe to Pipe

```
```



## TypeScript

- [ ] Why typed language?

```
search(term: string) : array[]{

    

}

```