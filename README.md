# NodeJS_Express_MySQL_at-localhost

// รันใช้ nodemon app.js
var express = require('express')
var cors = require('cors')
var bodyParser = require('body-parser')
var app = express()

//ใช้ libarly  ทำให้มีการจักการ body ที่มีการฝั่งข้อมูลมากับเส้น reqest
var jsonParser = bodyParser.json()

//ใช้ bcrypt ทำการเข้ารหรัสเพื่อความปลอดภัย
const bcrypt = require('bcrypt')
const saltRounds = 10

//ใช้ jwt สร้าง Token
var jwt = require('jsonwebtoken')
const secret ='react-jsonwebtoken'

//ใช้ jwt mysql2 เพื่อเข้าถึงฐานข้อมูล
const mysql = require('mysql2');
