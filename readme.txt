FGOSCCNT ver0.2.0 2020/4/3

Twitter @fgophi

FGO�X�N�V������A�C�e����CSV�o�͂���

�y�K�v�ȃ\�t�g�E�F�A�z
Python 3.7�ȍ~

�y�K�v�ȃ��C�u�����z
OpenCV
pageinfo.py https://github.com/max747/fgojunks/blob/master/pageinfo/pageinfo.py


�y�t�@�C���z
1. fgosccnt.py :���s�t�@�C��
2. makeitem.py item.xml ���쐬
3. makechest.py chest.xml ���쐬
4. makecard.py card.xml ���쐬
5. data �t�H���_ 2.3.4.�ŗp������t�@�C��
6. csv2counter.py (���܂�)fgosccnt.py�̏o��CSV��FGO����J�E���^�����ɂ���
7. qpsplit.py (���܂�)�X�N�V���t�@�C�����VQP���ƂɃt�H���_��������

�ȉ���2.3.4.���s���ɍ쐬�����
8. item.xml: �A�C�e�������̕�����ǂ�SVM�̃g���[�j���O�t�@�C��
9. chest.xml:  �h���b�v���̕�����ǂ�SVM�̃g���[�j���O�t�@�C��
10. card.xml:  �J�[�h�����̕�����ǂ�SVM�̃g���[�j���O�t�@�C��

�y�C���X�g�[���z
�EOpenCV ���C���X�g�[��
�Epageinfo.py �� fgosccnt.py �Ɠ���t�H���_���ɒu��
�Emakeitem.py, makechest.py, makecard.py �����ꂼ����s

��fgosccnt.py, item.xml chest.xml card.xml�𓯂��t�H���_�ɂ���邱��


�y�g�����z
usage: fgosccnt.py [-h] [--version] [filenames [filenames ...]]

FGO�X�N�V������A�C�e����CSV�o�͂���

positional arguments:
  filenames   ���̓t�@�C��

optional arguments:
  -h, --help  show this help message and exit
  --version   show program's version number and exit

�y���s���@�z
python fgosccnt.py �t�@�C��1 �t�@�C��2... > output.csv

�y����(��1)�z
filename,�󔠐�,item000001+1900,item000002x3,item000003x3,item000004
���v,26,3,3,22,1
IMG_2065.PNG,10,1,2,8,
IMG_2066.PNG,9,1,1,7,1
IMG_2067.PNG,7,1,,7,

�y����(��2)�z
filename,�󔠐�,QP+1900,��x3,����x3,�R�s
���v,26,3,3,22,1
IMG_2065.PNG,10,1,2,8,
IMG_2066.PNG,9,1,1,7,1
IMG_2067.PNG,7,1,,7,

�EVer0.7���험�i�����ɐ�����������Ă���ꍇ�A���̐�����F�����ďo�͂���
(�������{�[�i�X�\�L�͏Ȃ����)
���̂��ߗႦ��QP+1000��QP+1500�͓���item�t�@�C��1�ŔF�������
�Eitem �t�H���_�ɂł���t�@�C��.png�̃t�@�C�������A�C�e�����ɕύX����Ǝ�����s�ȍ~�����̃A�C�e�����ŕ\������邽�ߗ�2�̂悤�ɏo�͂���ǐ���������
�E�����ϊ����ꂽ��΂Ǝ����ϊ�����Ȃ���΂𓯂��A�C�e���Ƃ��ĔF���������ꍇ�̓t�H���_�𕪂��ē������O�̃A�C�e���t�@�C���ɂ���Γ������O�ŃJ�E���g�����
�E�S�������A�C�e���ŕʃt�@�C�����ł���ꍇ�����邪�A�t�H���_�𕪂��ē������O�̃A�C�e���t�@�C���ɂ���Γ������̂Ƃ��ăJ�E���g�����

�y�����z
2560x1600, 2436x1125, 2208x1242,2048x1536, 1920x1200, 1334x750�̉𑜓x�̂ݑΉ�
�E�S�������A�C�e���ł������̃A�C�e���t�@�C�����쐬����邱�Ƃ������H�ɂ���
�E���ɒ�𑜓x�̃X�N�V����JPEG���Ȃǂ̗򉻂�����ƌ듮�삵�₷���̂�PNG�̂܂܂̎g�p�𐄏�
�E�R�Ɖ΂̓f�[�^���������߂����炭��F�������

�y�����[�X�m�[�g�z

ver0.2
�E������OCR�̕i�����P
�E��΁E�P�΂̌�F���΍�
�E��΂̌�F���΍�
�E�h���b�v���\�L�����C�x���g�A�C�e���̌�F���΍�
�E�험�i���ԃ��[���ɂ�萳�����߂Â���C��

ver0.1.2
�E�험�i�̏��ԃ��[���̂�茵���Ȏ��s(�T�O�瑕�̃��A���e�B�͍l������Ȃ�)

ver0.1.1
�E�}�X�^�[�~�b�V�����̏��E�B���h�E�̂����Ńh���b�v�����ǂ߂Ȃ��o�O�̏C��
�EXML�t�@�C���̗e�ʂ��傫�����߁AGitHub�ň����Â炢�̂�makeitem.py makechest.py�Ŏg�p�҂��쐬����悤�ύX

ver0.1.0
�Epyocr�ATesseract OCR�Apillow���K�v�Ȃ��Ȃ���
�E�𑜓x���ƂɎ��s���𕪂���K�v�������Ȃ���
�E��x�̎��s�ŕ����̉𑜓x�̃X�N�V���̏������ł���悤�ɂȂ���
�E��݃A�C�e�����������ŔF������悤�ɂȂ���
�E�o��CSV�͏�݃A�C�e���Ɋւ��Ă͐험�i�̏��ԃ��[���ɏ]���ďo�͂����悤�ɂȂ���
�E�����t�@�C����F���������Ƃ���2�y�[�W�ȏ�ɂȂ���̂�2�y�[�W�ڈȍ~�������ꍇmissing�s���o�͂���悤�ɂȂ���

ver0.0.7
�E�험�i�̉����̐�����ǂ�ŏo�͂ł���悤�ɂ���

ver0.0.6
�E�A�C�e���g��F�����Ȃ��X�N�V���ɑΉ���������
�E�󔠐��⍇�v�����o�͂���悤�ɕύX
�E�󔠐�21�ȏ��4��ȏ�ɂȂ�험�i�̃X�N�V���ɑΉ�

ver0.0.5
�E�A�C�e���g��F�����Ȃ��X�N�V���ɑΉ���������
�E�����A�C�e���ňႤ���l�̏ꍇ�̌�F���̉��P
�EWindows����1�s�u���ɋ�s�������Ă��܂����̏C��

ver0.0.4
�E�摜�}�b�`���@�̏C���ɂ��F��������
�E������
�Eitem �f�B���N�g���͕K�����s�t�@�C���̂���f�B���N�g������T���悤�ɕύX
�E�摜�t�@�C����item �f�B���N�g���̃T�u�f�B���N�g������������悤�ɕύX

