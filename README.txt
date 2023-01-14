Creating new file 
    - ng g c filename
    - ng g c folder/filename

package: 
    - ng add @fortawesome/angular-fontawesome

------------------------>

    event emitter for reusable component and catch to another component
        *example:
            - a button should be use as reusable component 
            use @Output() btnClick = new EventEmitter(); 
            then declare it as btnClick.emit() to use and catch on another component
    Ref : https://www.youtube.com/watch?v=3dHNOWTI7H8&t=1834s (28:00)

ICONS
    - import { faTimes } from '@fortawesome/free-solid-svg-icons';
    - <fa-icon [ngStyle]="{ color: 'red' }" [icon]="faTimes"></fa-icon>

Observable 
    - to return as promise for asyncronous
    - import { Observable, of } from 'rxjs'
    - Observable<any> then declare as const any = of(any) then use subscribe(*like .then) to access
    *Note: we dont need this when you have http its automatically return as Observable

Http 
    - import { HttpClient, HttpHeaders } from '@angular/common/http';
    - declare the module on app.module.ts < import {HttpClientModule} from '@angular/common/http'
    - declare as private url = 'http://localhost:4200 
    - then declare on constructor as private http:HttpClient 
        -"http" can use now for get/post/put/delete

        *Note: dont need for "of" its return as Observable
    
    Ref : https://www.youtube.com/watch?v=3dHNOWTI7H8&t=1834s (1:01:41)
    Ref : https://www.youtube.com/watch?v=3dHNOWTI7H8&t=1834s (1:11:00) CRUD
    Ref : https://www.youtube.com/watch?v=3dHNOWTI7H8&t=1834s (1:19:00) HttpHeaders





