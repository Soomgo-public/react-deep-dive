# π€Ώ μ¨κ³ μ κ΅¬μ±μλ€κ³Ό ν¨κ»νλ React deep dive μ€ν°λ


## π₯ μ°Έκ³ μλ£

- [React.js Deep Dive Youtube Play List](https://www.youtube.com/watch?v=7YhdqIR2Yzo&list=PLxRVWC-K96b0ktvhd16l3xA6gncuGP7gJ)
    - React.js Deep Dive μ¬μλͺ©λ‘μ μλ 5κ°μ μμ

## π§­ μ΄μλ°©ν₯

```
1. μ€ν°λλ κ³΅μμ μΌλ‘ 10μ 27μΌλΆν° μμνλ©° λ§€μ£Ό λͺ©μμΌ 18μλΆν° 18μ 30λΆ κΉμ§ 30λΆλμ μ§ν
    - κ³΅μμ μΈ μκ° μ΄ν λ ν λ‘ νκ³  μΆμ κ²λ€μ΄ μλ μ¬λλ€μ λ¨μμ μμ λ‘­κ² ν λ‘ 
    - μ΄λ₯Ό μν΄ νμμκ°μ 1μκ°μΌλ‘ μμ½
2. λ§€μ£Ό λμκ°λ©΄μ λ¦¬λ©νλ νμ μ μ 
    - 30λΆμ μκ° μ€ 10λΆ μ λ μμνμ¬ μμμμ μΈκΈλλ νμμ μΈ λ΄μ©λ€ μμ£Όλ‘ μ€λͺ
    - 20λΆ μ λλ μλ‘ μμμ λ³΄λ©΄μ λλκ³  μΆμλ ν¬μΈνΈλ€μ λν΄ ν λ‘ 
    - κ³΅μμ μΈ μκ° μ΄νμ ν λ‘ μ μμ λ‘­κ² μ§ν
3. μ€ν°λ 1νλΉ μ€μ½₯
    - λ§€ ν μ μ°νκ² κ°μ Έκ°λ λ¦¬λ©νλ νμμ΄ λ¨Όμ  μ€ν°λ ν ν μ μ ν μ€μ½₯μ μ νμ¬ κ³΅μ 
```

## π μ€ν°λ μΌμ 

- λ§€μ£Ό λͺ©μμΌ 18:00 ~ 18:30 (#Room2)
    - μΊλ¦°λλ 1μκ°μΌλ‘ μ‘μλ (μ€ν°λ μ΄νμ ν λ‘ μ 1λ²λ°©μμ μ’ λ μμ λ‘­κ² ν  μ μκ² νκΈ° μν΄)

| μ£Όμ°¨  | μΌμ          | λΆλ                                                                                                                | μ°Έμ¬μ                                                                     |
|-----|-------------|-------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|
| 1μ£Όμ°¨ | 10μ 27μΌ (λͺ©) | How Does React Actually Work? React.js Deep Dive #1 (~5:33 React components, elements and component instances κΉμ§) | Holand, Keno, Zoey, **Ran**, Daniel, Jimmy, Collin
| 2μ£Όμ°¨ | 11μ 03μΌ (λͺ©) | How Does React Actually Work? React.js Deep Dive #1 (5:34 ~ 10:59 Reconciliation)                                 | **Holand**, Zoey, Ran, Jimmy
| 3μ£Όμ°¨ | 11μ 10μΌ (λͺ©) | How Does React Actually Work? React.js Deep Dive #1 (10:59 ~ Rendering)                                           | Holand, Zoey, Ran, **Jimmy**, Daniel, Harry, Keno
| 4μ£Όμ°¨ | 11μ 17μΌ (λͺ©) | What Is React Fiber? React.js Deep Dive #2                                                                        | Holand, **Zoey**, Jimmy, Daniel, Harry
| 5μ£Όμ°¨ | 11μ 24μΌ (λͺ©) | How Do React Hooks Actually Work? React.js Deep Dive #3                                                           | Zoey, Ran, **Harry**, Keno, Jimmy
| 6μ£Όμ°¨ | 12μ 01μΌ (λͺ©) | How Does React State Actually Work? React.js Deep Dive #4                                                         | Zoey, **Daniel**, Harry, Keno, Jimmy

## μ°Έμ¬μ :sparkles:

<table>
    <tr>
      <td align="center">
          <a href="https://github.com/dev-hikun">
              <img src="https://avatars0.githubusercontent.com/u/76590935?v=4" width="100;" alt="dev-hikun"/>
              <br />
              <sub><b>Harry</b></sub>
          </a>
      </td>
      <td align="center">
          <a href="https://github.com/jjm2317">
              <img src="https://avatars.githubusercontent.com/u/67041750?v=4" width="100;" alt="jjm2317"/>
              <br />
              <sub><b>Holand</b></sub>
          </a>
      </td>
      <td align="center">
          <a href="https://github.com/keoneokeoneo">
              <img src="https://avatars.githubusercontent.com/u/35859756?v=4" width="100;" alt="keoneokeoneo"/>
              <br />
              <sub><b>Keno</b></sub>
          </a>
      </td>
      <td align="center">
          <a href="https://github.com/Soyeon1128">
              <img src="https://avatars.githubusercontent.com/u/27682003?v=4" width="100;" alt="Soyeon1128"/>
              <br />
              <sub><b>Zoey</b></sub>
          </a>
      </td>
      <td align="center">
          <a href="https://github.com/seolranlee">
              <img src="https://avatars.githubusercontent.com/u/23238421?v=4" width="100;" alt="seolranlee"/>
              <br />
              <sub><b>Ran</b></sub>
          </a>
      </td>
      </tr>
      <tr>
      <td align="center">
          <a href="https://github.com/JinleeJeong">
              <img src="https://avatars.githubusercontent.com/u/45163013?v=4" width="100;" alt="JinleeJeong"/>
              <br />
              <sub><b>Daniel</b></sub>
          </a>
        </td>
        <td align="center">
            <a href="https://github.com/zeallat">
                <img src="https://avatars.githubusercontent.com/u/7078066?v=4" width="100;" alt="zeallat"/>
                <br />
                <sub><b>Jimmy</b></sub>
            </a>
        </td>
        <td align="center">
            <a href="https://github.com/flynnpark">
                <img src="https://avatars.githubusercontent.com/u/6476870?v=4" width="100;" alt="flynnpark"/>
                <br />
                <sub><b>Flynn</b></sub>
            </a>
        </td>
        <td align="center">
            <a href="https://github.com/colinmun">
                <img src="https://avatars.githubusercontent.com/u/86221372?v=4" width="100;" alt="colinmun"/>
                <br />
                <sub><b>Collin</b></sub>
            </a>
        </td>
    </tr>
</table>

