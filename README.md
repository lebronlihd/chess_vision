# SRTP_CNN_ChessBoardGenerating
SRTP_CNN_ChessBoardGenerating
new version

- 2021/06/16 versino 1.0
- 2021/10/30 final version 2.0
- Usage:
    - `init_mkdir.py` to create repo needed
    - `camera.py` for capturing images which are saved to `./test_image_process/systemCamTest`
    - `circle_crop.py` for croping chesses which are saved to `./test_image_process/image_circle_test`
    - Next step requires HUMAN to move cropped chesses to corresponding folder under `./data_pre_360`
    - `generate_data.py` to generate training data in `./data_360`
    - `trainModel.py` to train deep CNN models which are saved to `./model_save`
    - `circle_multi.py` to test the model using images in `./webcam`
    - `server_one.py` to run the chess vision TCP server for communication with Qt digital twin platform
- Environment:
    - python 3.6
    - tensorflow 2.4
    - keras 2.4
    - opencv
- Whole Structure

![Screenshot 2022-05-27 180653](https://user-images.githubusercontent.com/67775090/170679176-e01f23dd-6be9-42be-af77-70f440031236.png)

- DataGenerator

![1](https://github.com/LeBronLiHD/SRTP_CNN_ChessBoardGenerating/blob/master/chess_cnn/1.png)

- RedBlackReinforcement

![1](https://github.com/LeBronLiHD/SRTP_CNN_ChessBoardGenerating/blob/master/chess_cnn/2.png)

- RealChessboardImage

![2](https://github.com/LeBronLiHD/SRTP_CNN_ChessBoardGenerating/blob/master/chess_cnn/3.jpg)

- HoughCircleProcess

![2](https://github.com/LeBronLiHD/SRTP_CNN_ChessBoardGenerating/blob/master/chess_cnn/4.jpg)

- ChessLocationResult & ChessboardMatrixResult

![4](https://github.com/LeBronLiHD/SRTP_CNN_ChessBoardGenerating/blob/master/chess_cnn/5.png)
