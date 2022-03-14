## 1. First and last names 

***Andrey Gudin***

  ***Photo:***

  ![](https://lh3.googleusercontent.com/SaINbrs2weTpcwU1zrEERbND9cur2CuO2YU20JMe1-8jnBVecxxNCGeMn0H4WVOKGXQfntrjNDwk-dlpCjFguz0vyzTfuWG2RZZt0s7k6Cmf9dfUbJ5OgQFhezva2SaKvD0WehsCnw9RUV7fi7Rd1UI18NZHH-6AI4seWBxncKkyCf1SjhLyuHwoF3DVu5oh4kTMMeWMUlCcjnBgYCUXTFcaURid10yytSbQnkG1wCDbE0m8Ns0P4K4e6dAzsbKbS9OYeHjizl1DN63t3LRxKMAO4Hzo4iQQiyaA4HgJlCzWJGimfvnIdMErsLq6AAJ-L5SgCDDjH3Shrw-gz1lK2IVbizgOy4ystmOYgmOK7PhNzvbgazAIb1xGk9TDIdpPQjvhwHi0V-L1MuzrSO47ZpmFXaLRs2HbzqbbhuCXFBL4hIUDj_XfwaNfKfn_iI2YwwGIFTy3trpg1s6FOKw58j0uMRemZXGyOkMlKTUtayOtXaijGuk4I1R1d5M5AExj1eERqHN9KhibHJSpZ-M9nd58ouwMjLmeY0z5TkoVCcYlOwk0wX1eHXu2yWi02BOl8LZ0h9tYo9kY-Iql5uyO_S5WsUFUlomb780bElgK9iB9jdQizZzKwrCuCh45DD_-trPb2E7D1GuYAgtoCRd5zpW_fw7PRkcFoz32lzZTE_DEKyujMPF3fqjNrEJ6f86FdTwfbaAH32xJQDS0__kWuDO2=w793-h1057-no?authuser=0)


## 2. Contact information
   - Address: Russia Federation, Udmurt Republic, Sarapul
   - Phone: +79090604636
   - Email: aeon150791@gmail.com
   - GitHub: [AndreyGudin](https://github.com/AndreyGudin)
   - Discord: AndreyGudin(@andreygudin)

## 3. Brief information about me
My goal is to learn a new profession and find a job. I am currently working as a system administrator. I consider perseverance, love for learning new things, punctuality as my strengths.

## 4. Skills
   - HTML(template engine Pug)
   - CSS( preprocessor SCSS, BEM)
   - Javascript( beginner)
   - JQuery( beginner)
   - Version Control System : Git, GitHub
   - Module Bundler: WebPack
   - Figma
   - Code Editors: VS Code
   - Doker, Kybernetes, CI/CD( theory)

## 5. Code examples

```
function graphReviews(query = '.graph-reviews') {
    Chart.defaults.font.family =
      "Conv_Montserrat-Regular,Conv_Montserrat-Bold,Tahoma, Arial, sans-serif";
    const ctx = document.querySelector(`${query}__canvas`).getContext("2d");
    let gradient1 = ctx.createLinearGradient(54, 46, 54, 163);
    let gradient2 = ctx.createLinearGradient(120, 45, 120, 100);
    let gradient3 = ctx.createLinearGradient(110, 106, 110, 161);
    let gradient4 = ctx.createLinearGradient(100, 100, 100, 250);
    let gradient1Legend = ctx.createLinearGradient(182, 79, 182, 87);
    let gradient2Legend = ctx.createLinearGradient(182, 100, 182, 111);
    let gradient3Legend = ctx.createLinearGradient(182, 123, 182, 135);
    let gradient4Legend = ctx.createLinearGradient(182, 147, 182, 159);
    gradient1.addColorStop(0, "#FFE39C");
    gradient1.addColorStop(1, "#FFBA9C");
    gradient2.addColorStop(0, "#6FCF97");
    gradient2.addColorStop(1, "#66D2EA");
    gradient3.addColorStop(0, "#BC9CFF");
    gradient3.addColorStop(1, "#8BA4F9");
    gradient4.addColorStop(0, "#909090");
    gradient4.addColorStop(1, "#3D4975");
    gradient1Legend.addColorStop(0, "#FFE39C");
    gradient1Legend.addColorStop(1, "#FFBA9C");
    gradient2Legend.addColorStop(0, "#6FCF97");
    gradient2Legend.addColorStop(1, "#66D2EA");
    gradient3Legend.addColorStop(0, "#BC9CFF");
    gradient3Legend.addColorStop(1, "#8BA4F9");
    gradient4Legend.addColorStop(0, "#909090");
    gradient4Legend.addColorStop(1, "#3D4975");
    
    if ( screen.width <= 1230 ) {
      const myChart = new Chart(ctx, {
        type: "doughnut",
        data: {
          labels: ["Великолепно", "Хорошо", "Удовлетворительно", "Разочарован"],
          datasets: [
            {
              label: "My First Dataset",
              data: [130, 65, 65, 0],
              backgroundColor: [gradient1, gradient2, gradient3, gradient4],
            },
          ],
        },
        options: {
          cutout: "90%",
          radius: 60,
          maintainAspectRatio: false,
          rotation: 180,
          plugins: {
            legend: {
              display: true,
              position: "bottom",
              align: "start",
              maxWidth: 200,
              labels: {
                boxHeight: 10,
                boxWidth: 10,
                usePointStyle: true,
                pointStyle: "circle",
                font: {
                  size: 16,
                },
              },
            },
            title: {
              display: true,
              position: "top",
              text: "Впечатления от номера",
              font: {
                size: 19,
                family: "Conv_Montserrat-Bold",
              },
              padding: {
                bottom: 15,
              },
            },
          },
        },
        plugins: [
          {
            beforeDraw: function (c) {
              let legends = c.legend.legendItems;
              let gradients = [
                gradient1Legend,
                gradient2Legend,
                gradient3Legend,
                gradient4Legend,
              ];
              let i = 0;
              legends.forEach(function (e) {
                e.fillStyle = gradients[i];
                i++;
              });
            },
          },
        ],
      });
      myChart.update();
    } else {
      const myChart = new Chart(ctx, {
        type: "doughnut",
        data: {
          labels: ["Великолепно", "Хорошо", "Удовлетворительно", "Разочарован"],
          datasets: [
            {
              label: "My First Dataset",
              data: [130, 65, 65, 0],
              backgroundColor: [gradient1, gradient2, gradient3, gradient4],
            },
          ],
        },
        options: {
          cutout: "90%",
          radius: 60,
          maintainAspectRatio: false,
          rotation: 180,
          plugins: {
            legend: {
              display: true,
              position: "right",
              align: "end",
              maxWidth: 200,
              labels: {
                boxHeight: 10,
                boxWidth: 10,
                usePointStyle: true,
                pointStyle: "circle",
                font: {
                  size: 14,
                },
              },
            },
            title: {
              display: true,
              position: "top",
              text: "Впечатления от номера",
              font: {
                size: 19,
                family: "Conv_Montserrat-Bold",
              },
              padding: {
                bottom: 15,
              },
            },
          },
        },
        plugins: [
          {
            beforeDraw: function (c) {
              let legends = c.legend.legendItems;
              let gradients = [
                gradient1Legend,
                gradient2Legend,
                gradient3Legend,
                gradient4Legend,
              ];
              let i = 0;
              legends.forEach(function (e) {
                e.fillStyle = gradients[i];
                i++;
              });
            },
          },
        ],
      });
      myChart.update();
    }
}

export {graphReviews};
```


## 6. Work Experince

  [Hotel Site. Task 2 of Metalamp education, in process](https://github.com/AndreyGudin/project-metalamp2)


## 7. Education
  - Sarapul Polytechnic Institute
  - FreeCodeCamp(Responsive Web Design)
  - Metalamp( Second task)
  - Udemy: Полный курс по JavaScript + React - с нуля до результата,Docker Mastery: with Kubernetes +Swarm from a Docker Captain,Kubernetes Mastery: Hands-On Lessons From A Docker Captain


## 8. English
  [B1](https://examinator.epam.com/Main/PersonalAssignments/323312)
  