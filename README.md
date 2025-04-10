<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Certificado de Validação</title>
    <style>
        body {
            font-family: "Georgia", serif;
            background: #f8f8f8;
            padding: 40px;
        }
        .certificado {
            background: white;
            border: 2px solid #800000;
            padding: 40px;
            max-width: 800px;
            margin: auto;
            box-shadow: 0 0 15px rgba(0,0,0,0.2);
            position: relative;
        }
        .titulo {
            text-align: center;
            font-size: 28px;
            font-weight: bold;
            color: #800000;
            margin-bottom: 20px;
        }
        .logo {
            text-align: center;
            margin-bottom: 20px;
        }
        .logo img {
            max-height: 80px;
        }
        .info {
            font-size: 18px;
            line-height: 1.6;
        }
        .info span {
            font-weight: bold;
        }
        .footer {
            text-align: center;
            font-size: 12px;
            margin-top: 30px;
            color: #666;
        }
        .selo {
            position: absolute;
            right: 40px;
            top: 40px;
            background: #800000;
            color: white;
            padding: 10px 20px;
            font-weight: bold;
            transform: rotate(10deg);
        }
    </style>
</head>
<body>
    <div class="certificado">
        <div class="selo">Documento Válido</div>
        <div class="logo">
            <img src=https://github.com/user-attachments/assets/b3d5904c-2c4b-4aca-8ffc-efeca984036c alt="Universidade Cândido Mendes">
        </div>
        <div class="titulo">Certificado de Identificação Acadêmica</div>
        <div class="info">
            <p><span>Aluno:</span> Eduardo Seraphico de Souza Neto</p>
            <p><span>Curso:</span> Pós-Graduação em Processo Civil</p>
            <p><span>Matrícula:</span> 108020126</p>
            <p><span>CPF:</span> 128.624.587-75</p>
            <p><span>Data de Nascimento:</span> 30/10/1989</p>
            <p><span>Status:</span> Ativo</p>
        </div>
        <div class="footer">
            Consulta realizada em: <span id="timestamp"></span><br>
            Universidade Cândido Mendes – www.candidomendes.edu.br
        </div>
    </div>
    <script>
        const now = new Date();
        const formatDate = now.toLocaleString("pt-BR", { dateStyle: "short", timeStyle: "short" });
        document.getElementById("timestamp").textContent = formatDate;
    </script>
</body>
</html>
