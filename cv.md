# Artem Karlov

Beginner frontend developer 

## Contact
* __Home:__ Samara
* __Phone:__ +7 (927) 707-50-81 (preferred communication method)
* __Email:__ <ar.karlov@gmail.com>
* __Social:__
    * __GitHub:__ <https://github.com/ArtemKarlov>
    * __Telegram:__ [@arkarlov](https://t.me/arkarlov)

## Statement
I am considering changing my profession towards front-end development. I have no real work experience yet and the code examples are limited to assignments from online courses. Therefore, I am ready to complete the test task to show my ability for self-education and practical application of skills.

## Skills

#### Git
I know the Git commands at a basic level. I understand the difference between merge and rebase. In the process of work I use the "one commit, one task" approach. I can work with pull requests. 

#### HTML
I know at a basic level how to optimize loading CSS styles and JS scripts.  I am able to make up interfaces taking into account the built-in capabilities of the web platform:
* use special tags for page layout;
* pay attention to heading levels;
* checking access to all interactive elements using the keyboard. 

#### CSS
I use basic **BEM** principles when styling the page. I can create a responsive layout using **media expressions**. Most often, I use **flexbox** to position elements relative to each other. Have the basic knowledge to create transitions and animations. I know the CSS Frameworks: **Bootstrap**, **TailwindCSS** at a basic level. 

#### JavaScript
I know basic JS primitives, understand how to work with **Promise** and **async / await** syntax. I understand the difference between arrow functions and classical functions. I know how to restrict access to functions and variables using **closures**. When working with data, I try to use the modern capabilities of the language. 

#### OOP
I know the basic principles of object-oriented programming. 

#### React
I have a basic understanding of how React works. I know how to create applications using **Create React App**. I can:
* Create separate pages using **React Router**;
* Manage application state using **React Hooks**;
* Isolate component styles with **CSS Modules** and **Styled Components**.
Have basic knowledge of **redux** and **mobx**, but haven't applied it in practice yet.

#### Development environment
I use the **Visual Studio Code** editor with the **Prettier** plugin for easy code formatting. Familiar with **ESLint**. 

## Code examples

Example from Aviasales test poject: [GitHub repository](https://github.com/ArtemKarlov/Aviasales_test) ([gh-pages](https://artemkarlov.github.io/Aviasales_test/)):

* HTML
    ```html
    <!-- tickets -->
    <section id="tickets-section" class="tickets" data-item="tickets-section">
        <template id="ticket-template" data-item="ticket-template">
        <article class="tickets__item ticket">
            <header class="ticket__header">
            <span class="ticket__price" data-item="ticket-price">13&nbsp;400&nbsp;&#8381;</span>
            <div class="ticket__logo">
                <img src="img/S7 Logo.png" alt="carrier-logo" data-item="carrier-logo" class="carrier-logo"/>
            </div>
            </header>
            <template id="route-template" data-item="route-template">
            <div class="ticket__details ticket-route">
                <div class="ticket-route__details">
                <p class="ticket-route__label" data-item="route-title">MOW – HKT</p>
                <p class="ticket-route__value" data-item="route-time">10:45 – 08:00</p>
                </div>
                <div class="ticket-route__details">
                <p class="ticket-route__label">В пути</p>
                <p class="ticket-route__value" data-item="route-lenght">21ч 15м</p>
                </div>
                <div class="ticket-route__details">
                <p class="ticket-route__label" data-item="route-stops-count">
                    2 пересадки
                </p>
                <p class="ticket-route__value" data-item="route-stops">HKG, JNB</p>
                </div>
            </div>
            </template>
        </article>
        </template>
    </section>
    ```

* CSS
    ```css
    /* скрываем дефолтные инпуты */
    .input-default {
    position: absolute;
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
    outline: none;
    }

    .check-box {
    width: 100%;
    height: 40px;
    padding-left: 20px;
    padding-right: 20px;
    }

    /* меняем курсор на активных элементах */
    .check-box:hover,
    .sort-box__item:hover,
    .ticket:hover {
    cursor: url(img/Cursor.png), grab;
    }

    .check-box__text {
    font-size: 13px;
    line-height: 40px;
    margin-left: 30px;
    position: relative;
    }

    /* задаем кастомный чекбокс */
    .check-box__text::before {
    content: "";
    display: block;
    position: absolute;
    left: -30px;
    top: 50%;
    transform: translateY(-50%);
    width: 20px;
    height: 20px;
    border: 1px solid #9abbce;
    border-radius: 2px;
    }

    /* поведение при наведении и в фокусе  */
    .input-default_checkbox:focus + .check-box,
    .check-box:hover {
    background-color: #f1fcff;
    }

    .input-default_checkbox:checked + .check-box .check-box__text::before {
    border-color: #2196f3;
    background-image: url(img/Shape.png);
    background-repeat: no-repeat;
    background-position: center;
    }
    ```

* JavaScript
    ```javascript
    // выбираем билеты по количеству пересадок
    function getFilteredTickets(ticketsArray, ...filters) {
    if (filters.includes(FILTER_OPTION_ALL)) {
        return ticketsArray; //если выбран фильтр "все" - возвращаем весь массив билетов
    }
    const result = ticketsArray.filter((ticket) => {
        return filters.some((filter) => {
        return (
            ticket.segments.every((segment) => segment.stops.length <= filter) &&
            ticket.segments.some((segment) => segment.stops.length == filter)
        );
        });
    });

    return result;
    }
    ```

## Experience

**Student of front-end development courses** \
2020, *GeekBrains* \
Main practice projects:
* "HTML5 и CSS3" course: [GitHub repository](https://github.com/ArtemKarlov/GeekBrains-Waxom) ([gh-pages](https://artemkarlov.github.io/GeekBrains-Waxom/));
* "React JS" course: [GitHub repository](https://github.com/ArtemKarlov/GeekBrains-React);
* Soccer statistic test project: [GitHub repository](https://github.com/ArtemKarlov/soccer) ([gh-pages](https://artemkarlov.github.io/soccer/))
* Aviasales test poject: [GitHub repository](https://github.com/ArtemKarlov/Aviasales_test) ([gh-pages](https://artemkarlov.github.io/Aviasales_test/)).

**Deputy Head of the Laboratory of the Information Technology Department** \
2014 - 2020, *JSC "SIP RS"* \
Main responsibilities:
* design of corporate Structured Cabling;
* administration of a local network, servers;
* organization of purchases of computers and office equipment;
* installation and configuration of telecommunication equipment. 

**System Administrator** \
2012 - 2014,  *Ltd "Multi-Agent Technology"* \
Main responsibilities:
* administration of a local network, servers, PBX;
* maintenance of computers, office equipment;
* organization of purchases of computers and office equipment;
* user support. 



## Education

**Front-end developer** \
2020, *GeekBrains*, front-end development courses. 

**Candidate of Physico-Mathematical Sciences in Radiophysics**\
2016, *Samara State University*. 

**Professional computer technology developer**\
2011, *Samara State University*, honors degree. 

## Languages
* Russian - native;
* English - A2, elementary. I read technical documentation, periodically using Google Translate. 

## Hobbies

* Photography
* Sports
