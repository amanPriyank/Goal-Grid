1. How long did you spend on the coding test?

 I spent around 5 hours on the coding test. The task involved creating a 'To-Do' interface with essential features for managing, adding, editing, and deleting tasks. Additionally, I implemented search functionality and allowed users to set task priorities, with the option to search tasks by priority level. I took time to ensure the app functioned correctly, making adjustments as necessary based on my tests and observations.

2. What was the most useful feature that was added to the latest version of your chosen language? Please include a snippet of code that shows how you've used it.

 One of the most powerful feature of React is useEffect hooks. The useEffect Hook allows us to perform side effects in components. Here I've used this effec to store tasks concurrently in local storage.

  useEffect(() => {
    const todos = JSON.parse(localStorage.getItem("todos"));

    if (todos && todos.length > 0) {
      setTodos(todos);
    }
  }, []);
  

3. How would you track down a performance issue in production? Have you ever had to do this?

  a. I will create metrics and alarms to keep a monitor on health and performance of the app.
  b. If the performance goes below a certain level, alarm system will notify and I'll take the corrective measures to enhance the performance.
  c. Use database optimization techniques like, partioning, sharding and scaling according to the number of requests per second.
  d. Implement load balancer and consistent hashing techniques to make it more robust.
  e. I'll keep taking feedback from users and work for the betterment of the user experience.

  I've created metrics and alarms using prometheus client and created dashboard, uploaded it on Amazon Cloudwatch to monitor health and performance of the api when I was working in Amazon.

4. If you had more time, what additional features or improvements would you consider adding to the task management application?

  If I have been given more time I would have added these features:
  a. Connect it with database for storing tasks, deadlines and user profiles of multiple users.
  b. Implement authorization and authentication
  c. Add features like collaboration and chats with friends to create a healthy competitive environment among friends.
  d. Add notification for the upcoming deadlines of the tasks.