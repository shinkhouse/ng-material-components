## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { AfterContentInit } from '@angular/core';
import { AfterViewInit } from '@angular/core';
import { ChangeDetectorRef } from '@angular/core';
import { ControlValueAccessor } from '@angular/forms';
import { DoCheck } from '@angular/core';
import { ElementRef } from '@angular/core';
import { EventEmitter } from '@angular/core';
import { FocusMonitor } from '@angular/cdk/a11y';
import { FocusOrigin } from '@angular/cdk/a11y';
import * as i0 from '@angular/core';
import * as i1 from '@angular/material/core';
import * as i2 from '@angular/common';
import { InjectionToken } from '@angular/core';
import { OnDestroy } from '@angular/core';
import { OnInit } from '@angular/core';
import { QueryList } from '@angular/core';
import { ThemePalette } from '@angular/material/core';
import { UniqueSelectionDispatcher } from '@angular/cdk/collections';

// @public (undocumented)
export const MAT_RADIO_DEFAULT_OPTIONS: InjectionToken<MatRadioDefaultOptions>;

// @public (undocumented)
export function MAT_RADIO_DEFAULT_OPTIONS_FACTORY(): MatRadioDefaultOptions;

// @public
export const MAT_RADIO_GROUP: InjectionToken<MatRadioGroup>;

// @public
export const MAT_RADIO_GROUP_CONTROL_VALUE_ACCESSOR: any;

// @public (undocumented)
export class MatRadioButton implements OnInit, AfterViewInit, DoCheck, OnDestroy {
    constructor(radioGroup: MatRadioGroup, _elementRef: ElementRef, _changeDetector: ChangeDetectorRef, _focusMonitor: FocusMonitor, _radioDispatcher: UniqueSelectionDispatcher, animationMode?: string, _providerOverride?: MatRadioDefaultOptions | undefined, tabIndex?: string);
    ariaDescribedby: string;
    ariaLabel: string;
    ariaLabelledby: string;
    readonly change: EventEmitter<MatRadioChange>;
    get checked(): boolean;
    set checked(value: boolean);
    get color(): ThemePalette;
    set color(newValue: ThemePalette);
    get disabled(): boolean;
    set disabled(value: boolean);
    disableRipple: boolean;
    // (undocumented)
    protected _elementRef: ElementRef;
    focus(options?: FocusOptions, origin?: FocusOrigin): void;
    id: string;
    _inputElement: ElementRef<HTMLInputElement>;
    get inputId(): string;
    // (undocumented)
    _isRippleDisabled(): boolean;
    get labelPosition(): 'before' | 'after';
    set labelPosition(value: 'before' | 'after');
    _markForCheck(): void;
    name: string;
    // (undocumented)
    static ngAcceptInputType_checked: unknown;
    // (undocumented)
    static ngAcceptInputType_disabled: unknown;
    // (undocumented)
    static ngAcceptInputType_disableRipple: unknown;
    // (undocumented)
    static ngAcceptInputType_required: unknown;
    // (undocumented)
    static ngAcceptInputType_tabIndex: unknown;
    // (undocumented)
    ngAfterViewInit(): void;
    // (undocumented)
    ngDoCheck(): void;
    // (undocumented)
    ngOnDestroy(): void;
    // (undocumented)
    ngOnInit(): void;
    _noopAnimations: boolean;
    // (undocumented)
    _onInputClick(event: Event): void;
    _onInputInteraction(event: Event): void;
    _onTouchTargetClick(event: Event): void;
    radioGroup: MatRadioGroup;
    get required(): boolean;
    set required(value: boolean);
    protected _setDisabled(value: boolean): void;
    tabIndex: number;
    get value(): any;
    set value(value: any);
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatRadioButton, "mat-radio-button", ["matRadioButton"], { "id": { "alias": "id"; "required": false; }; "name": { "alias": "name"; "required": false; }; "ariaLabel": { "alias": "aria-label"; "required": false; }; "ariaLabelledby": { "alias": "aria-labelledby"; "required": false; }; "ariaDescribedby": { "alias": "aria-describedby"; "required": false; }; "disableRipple": { "alias": "disableRipple"; "required": false; }; "tabIndex": { "alias": "tabIndex"; "required": false; }; "checked": { "alias": "checked"; "required": false; }; "value": { "alias": "value"; "required": false; }; "labelPosition": { "alias": "labelPosition"; "required": false; }; "disabled": { "alias": "disabled"; "required": false; }; "required": { "alias": "required"; "required": false; }; "color": { "alias": "color"; "required": false; }; }, { "change": "change"; }, never, ["*"], true, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRadioButton, [{ optional: true; }, null, null, null, null, { optional: true; }, { optional: true; }, { attribute: "tabindex"; }]>;
}

// @public
export class MatRadioChange {
    constructor(
    source: MatRadioButton,
    value: any);
    source: MatRadioButton;
    value: any;
}

// @public (undocumented)
export interface MatRadioDefaultOptions {
    // (undocumented)
    color: ThemePalette;
}

// @public
export class MatRadioGroup implements AfterContentInit, OnDestroy, ControlValueAccessor {
    constructor(_changeDetector: ChangeDetectorRef);
    readonly change: EventEmitter<MatRadioChange>;
    // (undocumented)
    _checkSelectedRadioButton(): void;
    color: ThemePalette;
    _controlValueAccessorChangeFn: (value: any) => void;
    get disabled(): boolean;
    set disabled(value: boolean);
    _emitChangeEvent(): void;
    get labelPosition(): 'before' | 'after';
    set labelPosition(v: 'before' | 'after');
    // (undocumented)
    _markRadiosForCheck(): void;
    get name(): string;
    set name(value: string);
    // (undocumented)
    static ngAcceptInputType_disabled: unknown;
    // (undocumented)
    static ngAcceptInputType_required: unknown;
    ngAfterContentInit(): void;
    // (undocumented)
    ngOnDestroy(): void;
    onTouched: () => any;
    _radios: QueryList<MatRadioButton>;
    registerOnChange(fn: (value: any) => void): void;
    registerOnTouched(fn: any): void;
    get required(): boolean;
    set required(value: boolean);
    get selected(): MatRadioButton | null;
    set selected(selected: MatRadioButton | null);
    setDisabledState(isDisabled: boolean): void;
    _touch(): void;
    get value(): any;
    set value(newValue: any);
    writeValue(value: any): void;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<MatRadioGroup, "mat-radio-group", ["matRadioGroup"], { "color": { "alias": "color"; "required": false; }; "name": { "alias": "name"; "required": false; }; "labelPosition": { "alias": "labelPosition"; "required": false; }; "value": { "alias": "value"; "required": false; }; "selected": { "alias": "selected"; "required": false; }; "disabled": { "alias": "disabled"; "required": false; }; "required": { "alias": "required"; "required": false; }; }, { "change": "change"; }, ["_radios"], never, true, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRadioGroup, never>;
}

// @public (undocumented)
export class MatRadioModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRadioModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatRadioModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatRadioModule, never, [typeof i1.MatCommonModule, typeof i2.CommonModule, typeof i1.MatRippleModule, typeof i3.MatRadioGroup, typeof i3.MatRadioButton], [typeof i1.MatCommonModule, typeof i3.MatRadioGroup, typeof i3.MatRadioButton]>;
}

// (No @packageDocumentation comment for this package)

```
