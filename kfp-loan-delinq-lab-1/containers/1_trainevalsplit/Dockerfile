# Copyright 2018 The Kubeflow Authors
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM gcr.io/ml-pipeline/ml-pipeline-dataflow-tft:latest

RUN pip install -U scipy

RUN pip install -U numpy

RUN pip install -U scikit-learn

RUN pip install pandas

RUN pip install --upgrade google-cloud-storage

COPY . /

ENTRYPOINT ["python", "1_trainevalsplit/split_train_eval.py"]
