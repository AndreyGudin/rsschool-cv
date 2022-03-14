## 1. First and last names 

***Andrey Gudin***

  ***Photo:***

  ![](https://lh3.googleusercontent.com/WlPmtP-EaVNd4q1BGhzPtZcnIG3gROSabp17Dwsx6kJSnBfphbTwkdIYf_3Dqj9prk6ZJY7oAIaVyJ7i9QD41ffdyb8k6JfGX5p73T9FfsKxmCfvMieQGIScx37DJpozgwWtICEWI-lDXNSKlEdsMglMZRxu9uV_c76EOJNz17YrVV2wrr-LRWidVyt6_fE-_Y8J09KiA6fHqbSsg8ZqXuf2wZ9d05Pb-i6DXCpeWwlx9Y1REVCm9jbZAivkmF8RDDM36qmsdY2s1fUmDlI-j1WIcvxH8dxhr5-fXvtO31aivf-_jvpkDqnGUacdg6smBRgXNWlMayciAfPtygd6juLbMphR25JBwpYmsaLUVNpmygBW3_d5lxnztSewvHJJ-ccrxPTieLA3ggXRcFbpja_TDep-BLcmDY5g84guwxzRdn3X8Zpuc9TcTqNyhajK2L1AbISmxzbunvYd4WcDXgtZkvld9IkAa6WCGtTdGD4ryqC3A5_lzqZ4wVEFcDrcsWomJBcBL4t0i3WLMqjrBSwdHB87s-diI6NoEHd1u2kY05O-2Ji-F1OI0Wr155pnX-FExt0gV2SAryRAmcPwnC_cY5fSYMvvyMGdzvWmXgPXnk7LGMnvKXFsWRBAP6kOlnuy5eJo3SqUV8n901F1YR1yxh9jKVo3IjyBrOxm8h9oaxwfTjtYN0otsUe3eeDnfQMOMNoTOtsTURpIW-NSoez-=w750-h1000-no?authuser=0)


## 2. Contact information
   - ***Address***: Russian Federation, Udmurt Republic, Sarapul
   - ***Phone***: +79090604636
   - ***Email***: aeon150791@gmail.com
   - ***GitHub***: [AndreyGudin](https://github.com/AndreyGudin)
   - ***Discord***: AndreyGudin(@andreygudin)

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
  