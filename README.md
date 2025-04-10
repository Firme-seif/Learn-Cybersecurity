# Learn-Cybersecurity
تعلم الأمن السيبراني Learn Cybersecurity
<?php

use Illuminate\Support\Facades\Route;
use App\Http\Controllers\AwarenessController;
use App\Http\Controllers\TranslationController;
use App\Http\Controllers\AccessControlController;

// Route for Awareness Platform
Route::get('/awareness', [AwarenessController::class, 'index'])->name('awareness.index');

// Route for Translation Tool
Route::get('/translation', [TranslationController::class, 'index'])->name('translation.index');

// Route for Access Control System
Route::get('/access-control', [AccessControlController::class, 'index'])->name('access-control.index');<?php

namespace App\Http\Controllers;

use Illuminate\Http\Request;

class AwarenessController extends Controller
{
    public function index()
    {
        // Return the view for the Awareness Platform
        return view('awareness.index');
    }
}<?php

namespace App\Http\Controllers;

use Illuminate\Http\Request;

class TranslationController extends Controller
{
    public function index()
    {
        // Return the view for the Translation Tool
        return view('translation.index');
    }
}<?php

namespace App\Http\Controllers;

use Illuminate\Http\Request;

class AccessControlController extends Controller
{
    public function index()
    {
        // Return the view for the Access Control System
        return view('access-control.index');
    }
}<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة التوعية</title>
</head>
<body>
    <h1>مرحبًا بك في منصة التوعية!</h1>
    <p>هنا يمكنك التعرف على الأمن السيبراني باللغة العربية.</p>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أداة الترجمة</title>
</head>
<body>
    <h1>مرحبًا بك في أداة الترجمة!</h1>
    <p>قم بالبحث عن مصطلحات الأمن السيبراني هنا.</p>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>نظام إدارة الوصول</title>
</head>
<body>
    <h1>مرحبًا بك في نظام إدارة الوصول!</h1>
    <p>قم بإدارة صلاحيات المستخدمين هنا.</p>
</body>
</html>
