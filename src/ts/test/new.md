新测试用例

```ts
import { Component, DebugElement, ViewChild } from '@angular/core';
import { ComponentFixture, TestBed } from '@angular/core/testing';

describe('${1}', () => {
  let fixture: ComponentFixture<TestComponent>;
  let dl: DebugElement;
  let context: TestComponent;

  beforeEach(() => {
    TestBed.configureTestingModule({
      imports: [${2}],
      declarations: [TestComponent],
    });
    fixture = TestBed.createComponent(TestComponent);
    dl = fixture.debugElement;
    context = fixture.componentInstance;
    fixture.detectChanges();
  });

  $0
});

@Component({
  template: `
  <${3} #comp>
  </${3}>
  `,
})
class TestComponent {
  @ViewChild('comp') comp: ${4};
}
```