{\rtf1\ansi\ansicpg1252\cocoartf2822
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 @startuml\
left to right direction\
skinparam actorStyle awesome\
skinparam usecase \{\
  BackgroundColor #F0F8FF\
  BorderColor #2B3856\
\}\
\
actor "Usuario" as usuario #B0E0E6\
\
rectangle "Sistema Central" \{\
  (Autenticar usuario) as auth\
  (Registrar entidad) as registrar\
  (Consultar operaciones) as consultar\
  (Actualizar stock) as actualizar\
  (Generar reportes) as reportes\
\}\
\
usuario --> auth\
usuario --> registrar\
usuario --> consultar\
usuario --> actualizar\
usuario --> reportes\
\
@enduml}