step 1: cd backend
step 2: docker-compose up --build
step 3: login to ngrok & generate api token
step 4: open another terminal for ngrok
step 5: docker run -it -e NGROK_AUTHTOKEN=" enter your api key " ngrok/ngrok:latest http host.docker.internal:8000 
step 6: open another terminal for frontend
step 7: npm install 
step 8: for locally running ui, run command : npx expo start (for this will have to change theip address in App.tsx & api.ts to local ip address which can be obtained by ipconfig)
step 9: for creating tunnel, run command : npx expo start --tunnel ( ensure that the code has the ip address obtained from the ngrok pointing to the backend service)
