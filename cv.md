
# Nikita Kuzmin

## Frontend developer

### Contact Information:
* GitHub: SunkenRock21
* Email: kakoykakoy777@gmail.com
* Telegram: @SunkenRock21
* Vk.com: https://vk.com/sunken_rock

### About me:
Junior frontend developer (in progress), student at Rolling Scopes. I want to improve my programming skills and work in a team.

### Skills:
* HTML
* CSS
* Javascript
* Git
* BEM

### Сode Example:
```
function render() {
 
    tasksContainer.innerHTML = '';
    for (i = 0; i < taskArray.length; i++) {
    taskArray[i].id = i;
    tasksContainer.insertAdjacentHTML("beforeend", `<div id="task-${taskArray[i].id}" class="task"><div class="task-body"><button data-index="${taskArray[i].id}" class="task-checkbox"></button><p class="task-name">${taskArray[i].name}</p><p class="task-desc">${taskArray[i].desc}</p></div><button data-index="${taskArray[i].id}" class="task-edit-button"></button><button data-index="${taskArray[i].id}" class="task-delete-button"></button></div>`);
    let task = document.getElementById(`task-${taskArray[i].id}`);
    if (taskArray[i].completed == true) {
        task.classList.add("task__completed");
    } else if (taskArray[i].completed == false) {
        task.classList.remove("task__completed");
    }
    }
}
tasksContainer.onclick =  function(event) {
    let target = event.target;
    let attr = target.getAttribute("class");
    switch(attr) {
        case "task-delete-button":
            taskArray.splice(target.dataset.index, 1);
            break;
        case "task-edit-button":
            alert('edit');
            break;
        case "task-checkbox":
            if (taskArray[target.dataset.index].completed == false) {
                taskArray[target.dataset.index].completed = true;
            } else if (taskArray[target.dataset.index].completed == true) {
                taskArray[target.dataset.index].completed = false;}
            break;
    }
    render();
}

```
### Education:

The Rolling Scopes School- JavaScript/Front-end Course

### English level: 
B1
