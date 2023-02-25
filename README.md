# Домашнее задание к занятию "`8-03hw`" - `Ливчак Сергей`

---

### Задание 1

`Установка gitlab и настройка ранера в проекте "my_project"`

1. `Развернул виртуальную машину на локальном пк через vagrant на windows`
2. `Зарегестрировал runner "mashina-v-dokere"`

**Скриншот 1**
<img src = "img/Runner1.jpg" width = 100%>

**Скриншот 2**
<img src = "img/Runner1-2.jpg" width = 100%>

---

### Задание 2

`Копирование репозитория и исполнение pipeline`

1. `Нужно запушить скачаный репозиторий в свой gitlab`  
	В процессе столкнулся с тем что он увидел в моём гитлаб существующий
	проект (хоть и пустой), пришлось сделать 
	"git pull origin main --allow-unrelated-histories"
	"git push --set-upstream origin main"
2. `ссылка на пайплайн который я использовал для выполнения задания`  
	<[Gitlab-ci-original]> Сам не придумывал, взял из упражнения  


**Скриншот 3**  
<img src = "img/Pip1.jpg" width = 100%>  

**Скриншот 4**  
<img src = "img/Pip2.jpg" width = 85%>


---

### Задание 3

`Изменение Ci`

1. Изменил Ci так чтобы сборка происходила при изменении любых файлов кроме  
файлов с расширением ".go", а при изменении в файлах с расширением ".go" 
будет происходить вначале тест и только потом сборка
2. <[Gitlab-ci-modified]>


**Скриншот задания 3**
<img src = "img/git-modified-pipeline.jpg" width = 85%>



[Gitlab-ci-original]: https://github.com/Livchak/8-03hw/blob/main/original.gitlab-ci.yml
[Gitlab-ci-modified]: https://github.com/Livchak/8-03hw/blob/main/modified.gitlab-ci.yml