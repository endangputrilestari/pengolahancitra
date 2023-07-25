Nama  :Endang Putri Lestari
NIM   : 312110607
Kelas :TI.21.C.1



function varargout = contrast_stretch_and_histeq(varargin)
% CONTRAST_STRETCH_AND_HISTEQ MATLAB code for contrast_stretch_and_histeq.fig
%      CONTRAST_STRETCH_AND_HISTEQ, by itself, creates a new CONTRAST_STRETCH_AND_HISTEQ or raises the existing
%      singleton*.
%
%      H = CONTRAST_STRETCH_AND_HISTEQ returns the handle to a new CONTRAST_STRETCH_AND_HISTEQ or the handle to
%      the existing singleton*.
%
%      CONTRAST_STRETCH_AND_HISTEQ('CALLBACK',hObject,eventData,handles,...) calls the local
%      function named CALLBACK in CONTRAST_STRETCH_AND_HISTEQ.M with the given input arguments.
%
%      CONTRAST_STRETCH_AND_HISTEQ('Property','Value',...) creates a new CONTRAST_STRETCH_AND_HISTEQ or raises the
%      existing singleton*.  Starting from the left, property value pairs are
%      applied to the GUI before contrast_stretch_and_histeq_OpeningFcn gets called.  An
%      unrecognized property name or invalid value makes property application
%      stop.  All inputs are passed to contrast_stretch_and_histeq_OpeningFcn via varargin.
%
%      *See GUI Options on GUIDE's Tools menu.  Choose "GUI allows only one
%      instance to run (singleton)".
%
% See also: GUIDE, GUIDATA, GUIHANDLES
 
% Edit the above text to modify the response to help contrast_stretch_and_histeq
 
% Last Modified by GUIDE v2.5 12-Oct-2017 13:42:51
 
% Begin initialization code - DO NOT EDIT
gui_Singleton = 1;
gui_State = struct('gui_Name',       mfilename, ...
    'gui_Singleton',  gui_Singleton, ...
    'gui_OpeningFcn', @contrast_stretch_and_histeq_OpeningFcn, ...
    'gui_OutputFcn',  @contrast_stretch_and_histeq_OutputFcn, ...
    'gui_LayoutFcn',  [] , ...
    'gui_Callback',   []);
if nargin && ischar(varargin{1})
    gui_State.gui_Callback = str2func(varargin{1});
end
 
if nargout
    [varargout{1:nargout}] = gui_mainfcn(gui_State, varargin{:});
else
    gui_mainfcn(gui_State, varargin{:});
end
% End initialization code - DO NOT EDIT
 
% --- Executes just before contrast_stretch_and_histeq is made visible.
function contrast_stretch_and_histeq_OpeningFcn(hObject, eventdata, handles, varargin)
% This function has no output args, see OutputFcn.
% hObject    handle to figure
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
% varargin   command line arguments to contrast_stretch_and_histeq (see VARARGIN)
 
% Choose default command line output for contrast_stretch_and_histeq
handles.output = hObject;
 
% Update handles structure
guidata(hObject, handles);
movegui(hObject,'center');
 
% UIWAIT makes contrast_stretch_and_histeq wait for user response (see UIRESUME)
% uiwait(handles.figure1);
 
% --- Outputs from this function are returned to the command line.
function varargout = contrast_stretch_and_histeq_OutputFcn(hObject, eventdata, handles)
% varargout  cell array for returning output args (see VARARGOUT);
% hObject    handle to figure
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
 
% Get default command line output from handles structure
varargout{1} = handles.output;
 
function edit3_Callback(hObject, eventdata, handles)
% hObject    handle to edit3 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
 
% Hints: get(hObject,'String') returns contents of edit3 as text
%        str2double(get(hObject,'String')) returns contents of edit3 as a double
 
% --- Executes during object creation, after setting all properties.
function edit3_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit3 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called
 
% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end
 
function edit4_Callback(hObject, eventdata, handles)
% hObject    handle to edit4 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
 
% Hints: get(hObject,'String') returns contents of edit4 as text
%        str2double(get(hObject,'String')) returns contents of edit4 as a double
 
% --- Executes during object creation, after setting all properties.
function edit4_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit4 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called
 
% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end
 
function edit1_Callback(hObject, eventdata, handles)
% hObject    handle to edit1 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
 
% Hints: get(hObject,'String') returns contents of edit1 as text
%        str2double(get(hObject,'String')) returns contents of edit1 as a double
 
% --- Executes during object creation, after setting all properties.
function edit1_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit1 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called
 
% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end
 
function edit2_Callback(hObject, eventdata, handles)
% hObject    handle to edit2 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
 
% Hints: get(hObject,'String') returns contents of edit2 as text
%        str2double(get(hObject,'String')) returns contents of edit2 as a double
 
% --- Executes during object creation, after setting all properties.
function edit2_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit2 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called
 
% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end
 
% --- Executes on button press in pushbutton1.
function pushbutton1_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton1 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
[filename,pathname] = uigetfile('*.jpg');
 
if ~isequal(filename,0)
    Img = imread(fullfile(pathname,filename));
    axes(handles.axes1)
    imshow(Img)
    title('Original Image')
else
    return
end
 
handles.Img = Img;
guidata(hObject, handles)
 
% --- Executes on button press in pushbutton2.
function pushbutton2_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton2 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
Img = handles.Img;
 
Img_gray = rgb2gray(Img);
axes(handles.axes2)
imshow(Img_gray)
title('Grayscale')
 
axes(handles.axes3)
imhist(Img_gray)
title('Histogram')
grid on
 
handles.Img_gray = Img_gray;
guidata(hObject, handles)
 
% --- Executes on button press in pushbutton3.
function pushbutton3_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton3 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
Img_gray = handles.Img_gray;
Img_stretch = imstretch(Img_gray);
 
axes(handles.axes4)
imshow(Img_stretch)
title('Contrast Strecthing')
 
axes(handles.axes5)
imhist(Img_stretch)
title('Histogram')
grid on
 
[row,col] = size(Img_gray);
MSE = sum(sum((Img_stretch-Img_gray)^2))/(row*col);
PSNR = 10*log(1/MSE);
 
set(handles.edit1,'String',[PSNR,' dB']);
set(handles.edit2,'String',MSE);
 
% --- Executes on button press in pushbutton4.
function pushbutton4_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton4 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
Img_gray = handles.Img_gray;
Img_histeq = histogramequalization(Img_gray);
 
axes(handles.axes6)
imshow(Img_histeq)
title('Hist. Equalization')
 
axes(handles.axes7)
imhist(Img_histeq)
title('Histogram')
grid on
 
[row,col] = size(Img_gray);
MSE = sum(sum((Img_histeq-Img_gray)^2))/(row*col);
PSNR = 10*log(1/MSE);
 
set(handles.edit3,'String',[PSNR,' dB']);
set(handles.edit4,'String',MSE);
 
% --- Executes on button press in pushbutton5.
function pushbutton5_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton5 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
axes(handles.axes1)
cla reset
set(gca,'XTick',[])
set(gca,'YTick',[])
 
axes(handles.axes2)
cla reset
set(gca,'XTick',[])
set(gca,'YTick',[])
 
axes(handles.axes3)
cla reset
set(gca,'XTick',[])
set(gca,'YTick',[])
 
axes(handles.axes4)
cla reset
set(gca,'XTick',[])
set(gca,'YTick',[])
 
axes(handles.axes5)
cla reset
set(gca,'XTick',[])
set(gca,'YTick',[])
 
axes(handles.axes6)
cla reset
set(gca,'XTick',[])
set(gca,'YTick',[])
 
axes(handles.axes7)
cla reset
set(gca,'XTick',[])
set(gca,'YTick',[])
 
set(handles.edit1,'String',[])
set(handles.edit2,'String',[])
set(handles.edit3,'String',[])
set(handles.edit4,'String',[])
