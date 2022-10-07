# Oleksandr Shyhyda

## Contact Info
>- **Address:** Mykolaiv, Ukraine
>- **E-mail:** <bayanalex@gmail.com>
>- **LinkedIn:** [OleksandrShyhyda](https://www.linkedin.com/in/oleksandr-shyhyda-1150aa139)
>- **Telegram:** [@CyberAlex](https://t.me/CyberAlex)
>- **GitLab:** [cyberalex](https://gitlab.com/cyberalex)

---

## Summary

---

## Code example
**Codewars kata:** [Binomial Expansion](https://www.codewars.com/kata/540d0fdd3b6532e5c3000b5b)
```javascript
function expand(expr) {
    const a = +(expr.match(/(?<=\()-?\d*/).toString().replace(/-(?!\d)/, '-1') || '1');
    const b = +expr.match(/-?\d+(?=\))/).toString();
    const x = expr.match(/\w(?=[-+])/).toString();
    const n = +expr.match(/(?<=\^)\d+/).toString();
    let result = [];
    for(let k = n; k >= 0; k--) {
        let c = '' + (fact(n) / (fact(k) * fact(n - k))) * a**k * b**(n - k);
        if(c == '0')
            continue;  
        if(k != 0) {
            if(c == '1')
                c = '';
            else if (c == '-1')
                c = '-';
            c += k == 1 ? x : `${x}^${k}`;
        }
        result.push(c);
    }
    return result.join('+').replace(/\+-/g, '-');
  
    function fact(n) {
        if(n == 0)
            return 1;
        return n * fact(n - 1);
    }
}
```

---

## Education
>[**Admiral Makarov National University of Shipbuilding**](https://nuos.edu.ua/)  
>Master degree in *Electromechanical Systems and Electric Drive*  
>2005-2011  

---

## Work experience
>[**"A-Technologies" LLC**](http://a-technologies.com.ua/)  
>*Mykolaiv, Ukraine*  
>Marine radio and navagational equipment engineer  
>2011-...  

---

## Skills
>- **Computer**
>   * PC architecture
>   * Networking (basic)
>   * OS MS Windows, Linux (basic)
>   * MS Word, Excel, Outlook, PowerPoint
>- **Programming**
>   * Embedded C (Microchip PIC microcontrollers)
>   * Basic C++ (Qt)
>   * VBA (MS Word, Excel)
>   * __WEB (basic)__
>       + HTML
>       + CSS (SCSS, BEM naming)
>       + JavaScript
>   * GIT (basic)
> - **Electronics**
>   * Devices repair
>   * Schematic design
>   * Marine radio and navigational equipment installation and repair

---

## Courses
>- **Professional**
>   * **ECDIS by Transas (Wartsila)**  
>   *Istanbul, 2014; Gothenburg, 2018*
>   * **Inertial Navigational Systems by Teledyne TSS**  
>   *London, 2012*
>- **Web development**
>   * Markup [FreelancerLifeStyle](https://www.youtube.com/c/FreelancerLifeStyle/)
>   * JavaScript [learn.javascript.ru](https://learn.javascript.ru/)

---

## Languages
>- **Ukrainian** Native
>- **Russian** Fluent
>- **_English_** Upper Intermediate