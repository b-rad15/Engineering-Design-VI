# Lab 8
Create a new folder to run the examples 
```bash
python -m venv .venv
pip install scipy scikit-learn matplotlib pandas tensorflow keras
docker pull tensorflow/tensorflow
docker run -it tensorflow/tensorflow bash < "# apt update
apt full-upgrade \
apt install git-all \
git clone https://github.com/kevinwlu/iot.git \
pip install keras \
cd iot/lesson8 \
python keras_diabetes.py \
python keras_first_network.py \
pause \
exit"
```