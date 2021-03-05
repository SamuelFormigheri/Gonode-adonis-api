# Start Project

adonis new gonode --api-only

# ESLint

yarn add -D eslint
npx eslint --init

# Database

npm i --save sqlite3

# Controllers

adonis make:controller User
adonis make:controller Session
adonis make:controller ForgotPassword

# Mail

adonis install @adonisjs/mail

# Model

adonis make:model File -m -c  => -m cria migration -c cria controller
adonis make:model Project -m -c
adonis make:model Task -m -c

# Validator

adonis install @adonisjs/validator

adonis make:validator User

# Hook - "Event Listener"

adonis make:hook Task

# Redis

adonis install @adonisjs/redis

configuration on config/redis.js

# Adonis Kue

yarn add adonis-kue

# Jobs

create Jobs os app.js
adonis make:job NewTaskMail