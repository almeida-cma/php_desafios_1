<?php
// Inicia a sessão para armazenar as tarefas
session_start();

// Inicializa a lista de tarefas se não existir
if (!isset($_SESSION['tasks'])) {
    $_SESSION['tasks'] = [];
}

// Adiciona uma nova tarefa se o formulário for enviado
if ($_SERVER['REQUEST_METHOD'] === 'POST' && isset($_POST['task'])) {
    $newTask = trim($_POST['task']);
    if (!empty($newTask)) {
        $_SESSION['tasks'][] = $newTask;
    }
}

// Remove uma tarefa se o parâmetro de remoção for passado
if (isset($_GET['remove'])) {
    $taskIndex = (int)$_GET['remove'];
    if (isset($_SESSION['tasks'][$taskIndex])) {
        unset($_SESSION['tasks'][$taskIndex]);
        $_SESSION['tasks'] = array_values($_SESSION['tasks']); // Reindexa o array para evitar lacunas
    }

    // Redireciona para a página principal para evitar repetição do parâmetro "remove" na URL
    header("Location: " . $_SERVER['PHP_SELF']);
    exit();
}
?>

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lista de Tarefas - PHP</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
        }
        h1 {
            color: #333;
        }
        #taskInput {
            padding: 10px;
            width: 300px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        #addTaskButton {
            padding: 10px 20px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        #addTaskButton:hover {
            background-color: #218838;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        li {
            background-color: #fff;
            margin: 5px 0;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            display: flex;
            justify-content: space-between;
        }
        .removeTaskButton {
            background-color: #dc3545;
            color: white;
            border: none;
            padding: 5px 10px;
            border-radius: 4px;
            cursor: pointer;
        }
        .removeTaskButton:hover {
            background-color: #c82333;
        }
    </style>
</head>
<body>

    <h1>Lista de Tarefas</h1>

    <!-- Formulário para adicionar tarefas -->
    <form method="POST" action="">
        <input type="text" id="taskInput" name="task" placeholder="Digite sua tarefa...">
        <button type="submit" id="addTaskButton">Adicionar Tarefa</button>
    </form>

    <ul id="taskList">
        <?php
        // Verifica se há tarefas na sessão e as exibe
        if (!empty($_SESSION['tasks'])) {
            foreach ($_SESSION['tasks'] as $index => $task) {
                echo "<li>$task <a href='?remove=$index' class='removeTaskButton'>Remover</a></li>";
            }
        } else {
            echo "<li>Nenhuma tarefa adicionada.</li>";
        }
        ?>
    </ul>

</body>
</html>
