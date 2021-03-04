# Aleksey Kessler

### Contacts:
* **VK:** [https://vk.com/lesha_kessler](https://vk.com/lesha_kessler)
* **email**: [tov.kessler@yandex.ru](tov.kessler@yandex.ru)
* **GitHub**: [https://github.com/LightninG8/](https://github.com/LightninG8/)
### Short information:
I always strive for self-improvement. My main goal is to become a web development professional. I like programming. I can quickly learn new things, put into practice what I have previously learned, and start doing work long before the deadline. Also I can play three musical incstruments :). I worked for six months as a content manager in an online furniture store, developed a demo application in React.js for a project on online fitting of things, refined other people's websites, work a Junior frontend-developer in "ar-rocket" studio.

### Skills:
* HTML
* CSS + SASS/SCSS
* BEM methodology
* JavaScript (ES6)
* React.js + Redux
* Webpack
* Git

### Code example:
* Fetch data service
```
export default class Service {
    _apiBase = "http://localhost:8000";

    getResource = async (url) => {
        const res = await fetch(`${this._apiBase}${url}`);

        if (!res.ok) {
            throw new Error(`Could not fetch ${url} with status ${res.status}`);
        }

        return await res.json();
    }

    getMenuItems = async () => {
        return await this.getResource("/menu/");
    }
}
```
* React.js HOC bind service to component
```
    import React from 'react';
    import RestoServiceContext from '../resto-service-context';

    const withRestoService = () => (Wrapped) => {
        return (props) => {
            return (
                <RestoServiceContext.Consumer>
                    {
                        (RestoService) => {
                            return <Wrapped {...props} RestoService={RestoService}/>
                        }
                    }
                </RestoServiceContext.Consumer>
                
            )
        };
    };

    export default withRestoService;
```
### Experience
* React.js demo-application: [https://github.com/LightninG8/quiz-react-app](https://github.com/LightninG8/quiz-react-app)
* JavaScript MS paint app: [https://github.com/LightninG8/paint](https://github.com/LightninG8/paint)
* HTML, CSS, JavaScript landing: [https://github.com/LightninG8/waxom](https://github.com/LightninG8/waxom)

### Education
###### Cources:
* "Полный курс по JavaScript + React - с нуля до результата" Ivan Petrychenko
* "React JS Быстрый Курс 2020" Vladilen Minin
###### Books:
* "Don't make me think" Steve Krug
* "Современный учебник JavaScript" Ilya Kantor
###### Others:
* A lot of youtube videos of web-development

### English language
Level A2+
